---
title: Відсутні електронні листи в карантині
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831755"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ad9f7-102">Повідомлення електронної пошти відсутні в карантинах</span><span class="sxs-lookup"><span data-stu-id="ad9f7-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ad9f7-103">Адміністратори можуть [переглядати, випускати та видаляти ці повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ad9f7-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ad9f7-104">Щоб відкрити Центр безпеки &, перейдіть [https://protection.office.com](https://protection.office.com/) до .</span><span class="sxs-lookup"><span data-stu-id="ad9f7-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ad9f7-105">Щоб відкрити сторінку безпосередньо в карантин, перейдіть на сторінку [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ad9f7-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ad9f7-106">Ви можете шукати за такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="ad9f7-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ad9f7-107">**Ідентифікатор повідомлення:** глобальний унікальний ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ad9f7-108">Якщо вибрати повідомлення в списку, в **області** Відомості,  що з'явиться, з'явиться значення Ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ad9f7-109">Адміністратори можуть використовувати [трасування повідомлень,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) щоб знаходити повідомлення та відповідні значення ідентифікаторів повідомлень.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ad9f7-110">**Адреса електронної пошти відправника:** адреса електронної пошти одного відправника.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ad9f7-111">**Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ad9f7-112">**Тема**– використовуйте всю тему повідомлення.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ad9f7-113">У результатах пошуку не врагується регістр.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ad9f7-114">Ввівши умови пошуку, натисніть кнопку Оновити, щоб ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **відфільтрувати** результати.  </span><span class="sxs-lookup"><span data-stu-id="ad9f7-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ad9f7-115">Командлети, які використовуються для перегляду повідомлень і файлів і керування ними в карантині:</span><span class="sxs-lookup"><span data-stu-id="ad9f7-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ad9f7-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ad9f7-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ad9f7-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ad9f7-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ad9f7-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ad9f7-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ad9f7-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)зверніть увагу, що цей командлет призначено лише для повідомлень, які не призначено для зловмисних програм, які не підтримуються у службах SharePoint Online, "OneDrive для бізнесу" та Teams.</span><span class="sxs-lookup"><span data-stu-id="ad9f7-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ad9f7-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ad9f7-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)