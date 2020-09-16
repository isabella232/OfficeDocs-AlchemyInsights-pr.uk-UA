---
title: повне відновлення папки 1336
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741288"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="ff3f5-102">Повна папка "Відновлювані"</span><span class="sxs-lookup"><span data-stu-id="ff3f5-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="ff3f5-103">Для поштових скриньок Exchange Online стандартний граничний обсяг сховища для папки "Відновлювані" становить 30 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ff3f5-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="ff3f5-104">Граничний обсяг сховища для папки "Відновлювані елементи" автоматично збільшено до 100 ГБ, якщо поштова скринька поміщається на судове утримання, утримання eDiscovery або призначено політиці збереження.</span><span class="sxs-lookup"><span data-stu-id="ff3f5-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="ff3f5-105">Коли папка "Відновлювані" досягає граничного обсягу сховища, функція поштової скриньки впливає таким чином:</span><span class="sxs-lookup"><span data-stu-id="ff3f5-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="ff3f5-106">Користувач не може видаляти елемент із поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="ff3f5-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="ff3f5-107">Помічник із керованих папок не може видалити елемент на основі тега збереження або параметрів керованої папки.</span><span class="sxs-lookup"><span data-stu-id="ff3f5-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="ff3f5-108">Для поштових скриньок, у яких увімкнуто відновлення одного елемента або ввімкнуто, у процесі захисту від копіювання на сторінці не вдалося зберегти версії елементів, які ви редагуєте користувачем.</span><span class="sxs-lookup"><span data-stu-id="ff3f5-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="ff3f5-109">Для поштових скриньок, на яких ввімкнуто журналювання аудиту поштових скриньок, не можна зберігати записи журналів аудиту поштових скриньок у вкладеній папці "аудит" в папку "Відновлювані".</span><span class="sxs-lookup"><span data-stu-id="ff3f5-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="ff3f5-110">Для поштових скриньок, які не дотримуються, адміністратори можуть використовувати `Search-Mailbox -SearchDumpsterOnly -DeleteContent` команду в службі Exchange Online PowerShell, щоб видалити елементи в папці "Відновлювані елементи".</span><span class="sxs-lookup"><span data-stu-id="ff3f5-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="ff3f5-111">Щоб отримати докладніші відомості, ознайомтеся з такими темами:</span><span class="sxs-lookup"><span data-stu-id="ff3f5-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="ff3f5-112">Пошук і видалення повідомлень</span><span class="sxs-lookup"><span data-stu-id="ff3f5-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="ff3f5-113">Пошук у поштовій скриньці</span><span class="sxs-lookup"><span data-stu-id="ff3f5-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="ff3f5-114">Для поштових скриньок, які мають зберігатися, адміністратори повинні видалити утримання, перш ніж їх видалено з папки "Відновлювані елементи".</span><span class="sxs-lookup"><span data-stu-id="ff3f5-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="ff3f5-115">Докладні відомості наведено в статті [видалення елемента в папці "Відновлювані" в хмарних поштових скриньках у службі "утримання"](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="ff3f5-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="ff3f5-116">Щоб уникнути повної підтримки папки "Відновлювані елементи", адміністратори можуть збільшити граничний обсяг сховища для папки "Відновлювані" для поштових скриньок і настроїти політику збереження поштової скриньки, яка переміщає елементи з папки "Відновлювані елементи" до архівної поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="ff3f5-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="ff3f5-117">Див. [збільшення квоти на Відновлювані пункти для поштових скриньок у службі утримання](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="ff3f5-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
