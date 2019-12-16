---
title: Перевищено граничну кількість щоденних повідомлень електронної пошти. Робочий процес призупинено.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053138"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="354dc-103">Перевищено граничну кількість щоденних повідомлень електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="354dc-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="354dc-104">Робочий процес призупинено.</span><span class="sxs-lookup"><span data-stu-id="354dc-104">Workflow is suspended.</span></span>

<span data-ttu-id="354dc-105">Цю помилку можна отримати у таких випадках:</span><span class="sxs-lookup"><span data-stu-id="354dc-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="354dc-106">У вас є робочий цикл SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="354dc-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="354dc-107">Робочий цикл налаштовано на надсилання настроюваного повідомлення електронної пошти більш ніж 200 користувачів одночасно, більше 10 000 одержувачів на день або більше 30 повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="354dc-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="354dc-108">Під час запуску робочого циклу, повідомлення електронної пошти не надіслано, і ви помітите, що така поведінка:</span><span class="sxs-lookup"><span data-stu-id="354dc-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="354dc-109">Для робочого циклу, використовуючи тип платформи SharePoint 2013, перейдіть на сторінку **стан робочого циклу** .</span><span class="sxs-lookup"><span data-stu-id="354dc-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="354dc-110">На сторінці стан робочого циклу **внутрішній стан** налаштовано на **початок**, а інформаційна виноска **не може надіслати одержувачу**.</span><span class="sxs-lookup"><span data-stu-id="354dc-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="354dc-111">Щоб вирішити цю проблему, настройте робочий цикл для надсилання повідомлень електронної пошти без перевищення [меж відправника Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="354dc-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="354dc-112">Наприклад, використовуйте паузу в робочому циклі, надішліть повідомлення електронної пошти на групу Office 365, групу розсилки або поштову групу безпеки або надішліть повідомлення менше ніж 200 одержувачам одночасно.</span><span class="sxs-lookup"><span data-stu-id="354dc-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="354dc-113">Щоб отримати додаткові відомості, зверніться до такої [статті](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="354dc-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="354dc-114">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="354dc-114">Related topics</span></span>
- [<span data-ttu-id="354dc-115">Створити потік</span><span class="sxs-lookup"><span data-stu-id="354dc-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="354dc-116">SharePoint і Flow</span><span class="sxs-lookup"><span data-stu-id="354dc-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 