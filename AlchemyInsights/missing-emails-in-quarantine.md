---
title: Відсутні електронні листи в карантин
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569564"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="4b974-102">Відсутні електронні листи в карантин "</span><span class="sxs-lookup"><span data-stu-id="4b974-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="4b974-103">Адміністратори можуть [переглядати, випускати або видаляти ці повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="4b974-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="4b974-104">Щоб відкрити центр дотримання безпеки &, перейдіть до [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="4b974-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="4b974-105">Щоб відкрити сторінку карантину безпосередньо, перейдіть до [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="4b974-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="4b974-106">Можна виконати пошук за такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="4b974-106">You can search by the following values:</span></span>  

- <span data-ttu-id="4b974-107">**Ідентифікатор повідомлення**: глобальний унікальний ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4b974-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="4b974-108">Якщо у списку вибрано повідомлення, значення **ідентифікатора повідомлення** відобразиться в спливаючому вікні **відомостей** , що з'явиться.</span><span class="sxs-lookup"><span data-stu-id="4b974-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="4b974-109">Адміністратори можуть використовувати [трасування повідомлень](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) , щоб знайти повідомлення та їх ВІДПОВІДНІ значення ідентифікатора повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4b974-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="4b974-110">**Адреса електронної пошти відправника**: адреса електронної пошти одного відправника.</span><span class="sxs-lookup"><span data-stu-id="4b974-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="4b974-111">**Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.</span><span class="sxs-lookup"><span data-stu-id="4b974-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="4b974-112">**Тема**: використовуйте весь об'єкт повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4b974-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="4b974-113">Пошук не враховується з урахуванням регістру.</span><span class="sxs-lookup"><span data-stu-id="4b974-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="4b974-114">Після введення критеріїв пошуку натисніть ![ кнопку Оновити ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **оновлення** , щоб відфільтрувати результати.  </span><span class="sxs-lookup"><span data-stu-id="4b974-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="4b974-115">Командлети, які використовуються для перегляду та керування повідомленнями та файлами в карантин:</span><span class="sxs-lookup"><span data-stu-id="4b974-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="4b974-116">Видалити-карантин</span><span class="sxs-lookup"><span data-stu-id="4b974-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="4b974-117">Експорт-карантин</span><span class="sxs-lookup"><span data-stu-id="4b974-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="4b974-118">Отримати-карантин</span><span class="sxs-lookup"><span data-stu-id="4b974-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="4b974-119">[Попередній перегляд-карантин](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Зверніть увагу, що цей командлет призначений лише для повідомлень, а не зловмисних файлів з АТФ для SharePoint Online, OneDrive, для бізнесу або команди.</span><span class="sxs-lookup"><span data-stu-id="4b974-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="4b974-120">Реліз-карантин</span><span class="sxs-lookup"><span data-stu-id="4b974-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)