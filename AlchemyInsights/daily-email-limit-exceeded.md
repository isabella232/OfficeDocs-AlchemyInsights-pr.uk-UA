---
title: Email Ліміт добової перевищено. Робочий процес буде призупинено.
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
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059659"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="dff49-103">Щоденне електронне повідомлення вичерпана.</span><span class="sxs-lookup"><span data-stu-id="dff49-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="dff49-104">Робочий процес буде призупинено.</span><span class="sxs-lookup"><span data-stu-id="dff49-104">Workflow is suspended.</span></span>

<span data-ttu-id="dff49-105">Ця помилка може бути отримана в таких випадках:</span><span class="sxs-lookup"><span data-stu-id="dff49-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="dff49-106">У вас робочий процес у SharePoint Online, що використовує SharePoint 2010 або тип платформи робочого циклу SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="dff49-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="dff49-107">Робочий процес настроєний на надсилання повідомлення електронної пошти користувача більш ніж 200 користувачам час, більш ніж 10000 одержувачів на день або більше 30 повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="dff49-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="dff49-108">Під час запуску робочого процесу, не буде надіслано сповіщення електронною поштою, а ви помітили, що така поведінка:</span><span class="sxs-lookup"><span data-stu-id="dff49-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="dff49-109">Для робочого процесу за допомогою SharePoint 2013 тип платформи ви перейдіть до сторінки **Стану робочого процесу** .</span><span class="sxs-lookup"><span data-stu-id="dff49-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="dff49-110">На сторінці стану робочих **Started**встановлено **Внутрішній світ** і повітряна куля інформації відображає **не вдалося надіслати одержувачу**.</span><span class="sxs-lookup"><span data-stu-id="dff49-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="dff49-111">Щоб вирішити цю проблему, настройте робочий процес надсилання повідомлень електронної пошти без перевищення [Exchange Online відправника меж](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="dff49-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="dff49-112">Наприклад, використовуйте пауза робочого циклу, надіслати електронну пошту до Office 365 Група, групу розсилки або групу безпеки пошти ввімкнуто або відправити повідомлення до менше ніж 200 одержувачів одночасно.</span><span class="sxs-lookup"><span data-stu-id="dff49-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="dff49-113">Докладніше перегляньте наступні [статті](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="dff49-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="dff49-114">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="dff49-114">Related topics</span></span>
- [<span data-ttu-id="dff49-115">Створити потік</span><span class="sxs-lookup"><span data-stu-id="dff49-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="dff49-116">SharePoint і потік</span><span class="sxs-lookup"><span data-stu-id="dff49-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 