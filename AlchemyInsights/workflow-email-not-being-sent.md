---
title: Повідомлення електронної пошти робочого циклу не надсилатиметься
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749030"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="0a608-102">Повідомлення електронної пошти робочого циклу не надсилатиметься для списку або бібліотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="0a608-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="0a608-103">Повідомлення електронної пошти з робочих циклів не надсилатимуться всім користувачам або лише певним користувачам, або відображається повідомлення про помилку, **яке не можна надіслати. Переконайтеся, що в повідомленні електронної пошти є дійсний одержувач**.</span><span class="sxs-lookup"><span data-stu-id="0a608-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="0a608-104">Перевірте, чи є користувач у групі дозволи " **усі користувачі** " (список відомостей про користувачів) для цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="0a608-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="0a608-105">Зразок прямої URL-адреси: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/Peopl.aspx? Membershippid = 0</span><span class="sxs-lookup"><span data-stu-id="0a608-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="0a608-106">Якщо користувач не існує, переконайтеся, що користувач ввійшов до сторінки.</span><span class="sxs-lookup"><span data-stu-id="0a608-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="0a608-107">Якщо це зовнішній користувач, переконайтеся, що їх запрошення прийнято.</span><span class="sxs-lookup"><span data-stu-id="0a608-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="0a608-108">Якщо користувач існує у групі дозволи, переконайтеся, що адреса електронної пошти правильна.</span><span class="sxs-lookup"><span data-stu-id="0a608-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="0a608-109">Якщо адресу електронної пошти користувачів не настроєно, а потім створіть зразок оповіщення для цього користувача, який примусово синхронізує цей обліковий запис користувача від профілів користувачів SharePoint до цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="0a608-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="0a608-110">Електронна пошта від робочих циклів надсилатиметься адміністраторам колекції сайтів, але не до інших користувачів і не бачить помилку **http, забороненої <span>https:</span>//url/_vti_bin/Client.xvc.SP.utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="0a608-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="0a608-111">Переглянути [відмовлено в доступі під час надсилання повідомлення електронної пошти групі SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="0a608-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="0a608-112">Крім того, переконайтеся, що функція " **режим блокування дозволів користувачів із обмеженим доступом** " не активна.</span><span class="sxs-lookup"><span data-stu-id="0a608-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="0a608-113">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="0a608-113">Related topics</span></span>
<span data-ttu-id="0a608-114">Хочете спробувати Microsoft Flow у службі SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="0a608-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="0a608-115">Створення потоку</span><span class="sxs-lookup"><span data-stu-id="0a608-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0a608-116">SharePoint і передавання</span><span class="sxs-lookup"><span data-stu-id="0a608-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


