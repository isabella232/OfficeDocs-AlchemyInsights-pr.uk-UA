---
title: Робочий процес не надіслане
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530912"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="78557-102">Робочий процес не надіслане для списку або бібліотеки</span><span class="sxs-lookup"><span data-stu-id="78557-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="78557-103">Лист від робочі процеси не надсилаються до всіх користувачів, або лише певним користувачам, або ви бачите помилку **повідомлення електронної пошти не може бути надіслано. Переконайтеся, що електронна пошта має непридатне**.</span><span class="sxs-lookup"><span data-stu-id="78557-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="78557-104">Перевірте, якщо користувач існує у **Всіх людей** дозволи групі (списку відомостей про користувача) для цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="78557-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="78557-105">Скуштуйте прямій URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="78557-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="78557-106">Якщо користувач не існує, переконайтеся, що користувач буде підписано в сторінку.</span><span class="sxs-lookup"><span data-stu-id="78557-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="78557-107">Якщо це із зовнішнім користувачем, переконайтеся, що їх запрошення було прийнято.</span><span class="sxs-lookup"><span data-stu-id="78557-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="78557-108">Якщо користувач дійсно існує у групі дозволи, переконайтеся, що адреса електронної пошти правильна.</span><span class="sxs-lookup"><span data-stu-id="78557-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="78557-109">Якщо адреси електронної пошти користувачів не тут, потім створити зразок оповіщення для цього користувача, який змушує синхронізацію цього облікового запису користувача із профілів користувачів SharePoint для цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="78557-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="78557-110">Лист від робочі процеси надсилаються адміністраторам колекції сайтів, а не іншим користувачам і бачити помилки **HTTP Заборонене до <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="78557-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="78557-111">Переглянути [Доступ заборонено під час надсилання повідомлення електронної пошти до групи SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="78557-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="78557-112">Крім того, переконайтеся, що **режим обмеженим доступом користувача дозволу lockdown** функції колекції сайтів не є активним.</span><span class="sxs-lookup"><span data-stu-id="78557-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="78557-113">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="78557-113">Related topics</span></span>
<span data-ttu-id="78557-114">Хочете спробувати Microsoft потік в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="78557-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="78557-115">Створити потік</span><span class="sxs-lookup"><span data-stu-id="78557-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="78557-116">SharePoint і потік</span><span class="sxs-lookup"><span data-stu-id="78557-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


