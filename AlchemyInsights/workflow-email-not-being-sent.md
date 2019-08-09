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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270693"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="1f996-102">Робочий процес не надіслане</span><span class="sxs-lookup"><span data-stu-id="1f996-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="1f996-103">Лист від робочі процеси не надсилаються до всіх користувачів, або лише певним користувачам, або ви бачите помилку **повідомлення електронної пошти не може бути надіслано. Переконайтеся, що електронна пошта має непридатне**.</span><span class="sxs-lookup"><span data-stu-id="1f996-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="1f996-104">Перевірте, якщо користувач існує у **Всіх людей** дозволи групі (списку відомостей про користувача) для цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="1f996-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1f996-105">Скуштуйте прямій URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1f996-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="1f996-106">Якщо користувач не існує, переконайтеся, що користувач буде підписано в сторінку.</span><span class="sxs-lookup"><span data-stu-id="1f996-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="1f996-107">Якщо це із зовнішнім користувачем, переконайтеся, що їх запрошення було прийнято.</span><span class="sxs-lookup"><span data-stu-id="1f996-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="1f996-108">Якщо користувач дійсно існує у групі дозволи, переконайтеся, що адреса електронної пошти правильна.</span><span class="sxs-lookup"><span data-stu-id="1f996-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="1f996-109">Якщо адреси електронної пошти користувачів не тут, потім створити зразок оповіщення для цього користувача, який змушує синхронізацію цього облікового запису користувача із профілів користувачів SharePoint для цієї колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="1f996-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1f996-110">Лист від робочі процеси надсилаються адміністраторам колекції сайтів, а не іншим користувачам і бачити помилки \*\*HTTP Заборонене до <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="1f996-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="1f996-111">Подивитися [Відмовлено в доступі коли послав електронну пошту, групи](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="1f996-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="1f996-112">Крім того, переконайтеся, що **режим обмеженим доступом користувача дозволу lockdown** функції колекції сайтів не є активним.</span><span class="sxs-lookup"><span data-stu-id="1f996-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="1f996-113">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="1f996-113">Related topics</span></span>
<span data-ttu-id="1f996-114">Хочете спробувати Microsoft потік в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="1f996-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1f996-115">Створити потік</span><span class="sxs-lookup"><span data-stu-id="1f996-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1f996-116">SharePoint і потік</span><span class="sxs-lookup"><span data-stu-id="1f996-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


