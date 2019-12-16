---
title: Електронна пошта робочого циклу не надсилаються
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049394"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="e0042-102">Електронна пошта робочого циклу не надсилається до списку або бібліотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="e0042-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="e0042-103">Повідомлення електронної пошти з робочих циклів не надсилаються всім користувачам або лише певним користувачам, або відображається повідомлення про помилку, **яке не вдалося надіслати. Переконайтеся, що повідомлення електронної пошти має дійсний одержувач**.</span><span class="sxs-lookup"><span data-stu-id="e0042-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="e0042-104">Перевірте, чи існує користувач у групі дозволи **всіх** користувачів (список відомостей про користувача) для цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="e0042-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="e0042-105">Приклад прямої URL-адреси<tenant>: https://<sitename>. SharePoint.com/Sites//_layouts/15/Car.GRA? Членпідкод = 0</span><span class="sxs-lookup"><span data-stu-id="e0042-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="e0042-106">Якщо користувач не існує, переконайтеся, що користувач увійшов до сторінки.</span><span class="sxs-lookup"><span data-stu-id="e0042-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="e0042-107">Якщо це зовнішній користувач, переконайтеся, що їхнє запрошення прийняте.</span><span class="sxs-lookup"><span data-stu-id="e0042-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="e0042-108">Якщо користувач існує у групі дозволів, переконайтеся, що адреса електронної пошти правильна.</span><span class="sxs-lookup"><span data-stu-id="e0042-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="e0042-109">Якщо тут не встановлено адресу електронної пошти користувачів, створіть зразок оповіщення для цього користувача, який примушує синхронізацію цього облікового запису користувача з профілів користувачів SharePoint до цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="e0042-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="e0042-110">Повідомлення електронної пошти з робочих циклів надсилаються адміністраторам колекції сайтів, але не іншим користувачам і відображається повідомлення про помилку **http заборонено <span>https:</span>//URL/_vti_bin/Client.xvc.SP.utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="e0042-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="e0042-111">Переглянути [відмовлено в доступі під час надсилання повідомлення електронної пошти до групи SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="e0042-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="e0042-112">Крім того, переконайтеся, що функція **доступу до прав користувачів із обмеженим доступом до режиму блокування** сайтів не активна.</span><span class="sxs-lookup"><span data-stu-id="e0042-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="e0042-113">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="e0042-113">Related topics</span></span>
<span data-ttu-id="e0042-114">Бажаєте спробувати Microsoft Flow у SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e0042-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e0042-115">Створити потік</span><span class="sxs-lookup"><span data-stu-id="e0042-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e0042-116">SharePoint і Flow</span><span class="sxs-lookup"><span data-stu-id="e0042-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


