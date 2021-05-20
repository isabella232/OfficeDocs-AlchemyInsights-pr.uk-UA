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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539845"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="4841a-102">Повідомлення електронної пошти відсутні в карантинах</span><span class="sxs-lookup"><span data-stu-id="4841a-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="4841a-103">Адміністратори можуть [переглядати, випускати та видаляти ці повідомлення.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="4841a-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="4841a-104">Щоб відкрити Центр безпеки &, перейдіть [https://protection.office.com](https://protection.office.com/) до .</span><span class="sxs-lookup"><span data-stu-id="4841a-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="4841a-105">Щоб відкрити сторінку безпосередньо в карантин, перейдіть на сторінку [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="4841a-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="4841a-106">Ви можете шукати за такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="4841a-106">You can search by the following values:</span></span>  

- <span data-ttu-id="4841a-107">**Ідентифікатор повідомлення:** глобальний унікальний ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4841a-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="4841a-108">Якщо вибрати повідомлення в списку, в **області** Відомості,  що з'явиться, з'явиться значення Ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4841a-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="4841a-109">Адміністратори можуть використовувати [трасування повідомлень,](/microsoft-365/security/office-365-security/message-trace-scc) щоб знаходити повідомлення та відповідні значення ідентифікаторів повідомлень.</span><span class="sxs-lookup"><span data-stu-id="4841a-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="4841a-110">**Адреса електронної пошти відправника:** адреса електронної пошти одного відправника.</span><span class="sxs-lookup"><span data-stu-id="4841a-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="4841a-111">**Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.</span><span class="sxs-lookup"><span data-stu-id="4841a-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="4841a-112">**Тема**– використовуйте всю тему повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4841a-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="4841a-113">У результатах пошуку не врагується регістр.</span><span class="sxs-lookup"><span data-stu-id="4841a-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="4841a-114">Ввівши умови пошуку, натисніть кнопку Оновити, щоб ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **відфільтрувати** результати.</span><span class="sxs-lookup"><span data-stu-id="4841a-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="4841a-115">Командлети, які використовуються для перегляду повідомлень і файлів і керування ними в карантині:</span><span class="sxs-lookup"><span data-stu-id="4841a-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="4841a-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4841a-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="4841a-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4841a-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="4841a-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4841a-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="4841a-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)зверніть увагу, що цей командлет доступний лише для повідомлень, а не файлів зі зловмисних програм із Microsoft Defender для Office 365 для SharePoint Online, OneDrive для бізнесу або Teams.</span><span class="sxs-lookup"><span data-stu-id="4841a-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="4841a-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4841a-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)