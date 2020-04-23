---
title: 1336 відновлення папки елементів заповнено
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720273"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="1e36a-102">Папка «Відновлювані елементи» заповнено</span><span class="sxs-lookup"><span data-stu-id="1e36a-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="1e36a-103">Для поштових скриньок Exchange Online обмеження сховища за промовчанням для папки «Відновлювані» становить 30 ГБ.</span><span class="sxs-lookup"><span data-stu-id="1e36a-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="1e36a-104">Граничний обсяг сховища для папки «Відновлювані елементи» автоматично збільшується до 100 ГБ, якщо поштова скринька розміщується на судовому утриманні, пошук необхідної інформації, або призначається політиці збереження.</span><span class="sxs-lookup"><span data-stu-id="1e36a-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="1e36a-105">Після того, як Відновлювані елементи папки, досягає обмеження на зберігання, функції поштової скриньки, що впливає таким чином:</span><span class="sxs-lookup"><span data-stu-id="1e36a-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="1e36a-106">Користувач не може видалити елементи з поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="1e36a-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="1e36a-107">Помічник із керованих папок не може видалити елементи на основі тегу збереження або параметрів керованих папок.</span><span class="sxs-lookup"><span data-stu-id="1e36a-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="1e36a-108">Для поштових скриньок, які мають один елемент відновлення ввімкнуто, або розміщені на утримання, копіювання та записування сторінки процес захисту не може підтримувати версії елементів, які редагується користувачем.</span><span class="sxs-lookup"><span data-stu-id="1e36a-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="1e36a-109">Для поштових скриньок, які мають журналювання аудиту поштової скриньки, не можна зберегти записи журналу аудиту поштової скриньки в папці «Відновлювані» папки перевірки.</span><span class="sxs-lookup"><span data-stu-id="1e36a-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="1e36a-110">Для поштових скриньок, які не є утримувані, адміністратори `Search-Mailbox -SearchDumpsterOnly -DeleteContent` можуть використовувати команду в Exchange Online PowerShell для видалення елементів у папці «Відновлювані елементи».</span><span class="sxs-lookup"><span data-stu-id="1e36a-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="1e36a-111">Для отримання додаткових відомостей зверніться до таких розділів:</span><span class="sxs-lookup"><span data-stu-id="1e36a-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="1e36a-112">Як шукати й видаляти повідомлення</span><span class="sxs-lookup"><span data-stu-id="1e36a-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="1e36a-113">Пошук-поштову скриньку</span><span class="sxs-lookup"><span data-stu-id="1e36a-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="1e36a-114">Для поштових скриньок, які знаходяться на утриманні, адміністратори повинні видалити утримання, перш ніж вони зможуть видалити елементи з папки "Відновлювані".</span><span class="sxs-lookup"><span data-stu-id="1e36a-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="1e36a-115">Для отримання додаткових відомостей див. [видалення елементів у папці «Відновлювані елементи» на основі хмарних поштових скриньок](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="1e36a-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="1e36a-116">Щоб запобігти повному відновленню папки «Відновлювані», адміністратори можуть збільшити обмеження сховища для папки «Відновлювані» для поштових скриньок, які потрібно утримувати, і настроїти політику збереження поштової скриньки, яка переміщує елементи з папки «Відновлювані елементи» до архівної поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="1e36a-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="1e36a-117">Переглянути [, як збільшити квоту видобутих елементів для поштових скриньок](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold), які призупинено.</span><span class="sxs-lookup"><span data-stu-id="1e36a-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
