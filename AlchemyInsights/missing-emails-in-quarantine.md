---
title: Відсутні повідомлення електронної пошти в карантині
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673735"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ce18e-102">Відсутні повідомлення електронної пошти в карантині "</span><span class="sxs-lookup"><span data-stu-id="ce18e-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ce18e-103">Адміністратори можуть [переглядати, вивільняти або видаляти ці повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ce18e-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ce18e-104">Щоб відкрити центр відповідності & безпеки, перейдіть до розділу [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="ce18e-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ce18e-105">Щоб відкрити сторінку карантину безпосередньо, перейдіть до [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ce18e-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ce18e-106">Шукати можна за такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="ce18e-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ce18e-107">**Ідентифікатор повідомлення**: глобальний унікальний ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="ce18e-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ce18e-108">Якщо ви вибрали повідомлення в списку, то в області " **докладно** ", що Відкриється, ВІДОБРАЖАЄТЬСЯ значення **ідентифікатора повідомлення** .</span><span class="sxs-lookup"><span data-stu-id="ce18e-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ce18e-109">Адміністратори можуть використовувати [трасування повідомлень](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) , щоб знаходити повідомлення та відповідні значення ідентифікаторів повідомлень.</span><span class="sxs-lookup"><span data-stu-id="ce18e-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ce18e-110">**Адреса електронної пошти відправника**: адреса електронної пошти одного відправника.</span><span class="sxs-lookup"><span data-stu-id="ce18e-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ce18e-111">**Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.</span><span class="sxs-lookup"><span data-stu-id="ce18e-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ce18e-112">**Тема**: використайте всю тему повідомлення.</span><span class="sxs-lookup"><span data-stu-id="ce18e-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ce18e-113">Пошук не враховує регістр.</span><span class="sxs-lookup"><span data-stu-id="ce18e-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ce18e-114">Ввівши умови пошуку, натисніть кнопку Оновити, ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** щоб відфільтрувати результати.  </span><span class="sxs-lookup"><span data-stu-id="ce18e-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ce18e-115">Командлети, які використовуються для перегляду та керування повідомленнями та файлами в карантині:</span><span class="sxs-lookup"><span data-stu-id="ce18e-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ce18e-116">Видалення – карантин</span><span class="sxs-lookup"><span data-stu-id="ce18e-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ce18e-117">Експорт – карантин</span><span class="sxs-lookup"><span data-stu-id="ce18e-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ce18e-118">Початок-карантин</span><span class="sxs-lookup"><span data-stu-id="ce18e-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ce18e-119">[Ознайомлювальну версію – карантин](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Зауважте, що цей командлет призначено лише для повідомлень, а не зловмисних файлів із АТФ для служби SharePoint Online, OneDrive для бізнесу або робочих груп.</span><span class="sxs-lookup"><span data-stu-id="ce18e-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ce18e-120">Випуск – карантин</span><span class="sxs-lookup"><span data-stu-id="ce18e-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)