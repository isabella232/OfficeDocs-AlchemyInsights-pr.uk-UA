---
title: Перевищено граничний обсяг щоденного повідомлення електронної пошти. Робочий цикл призупинено.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731584"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="5d7f9-103">Перевищено граничний обсяг щоденного повідомлення електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="5d7f9-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="5d7f9-104">Робочий цикл призупинено.</span><span class="sxs-lookup"><span data-stu-id="5d7f9-104">Workflow is suspended.</span></span>

<span data-ttu-id="5d7f9-105">Цю помилку можна отримати в таких ситуаціях:</span><span class="sxs-lookup"><span data-stu-id="5d7f9-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="5d7f9-106">Ви маєте робочий цикл у службі SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="5d7f9-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="5d7f9-107">Робочий цикл настроєно для надсилання настроюваного повідомлення електронної пошти для більш ніж 200 користувачів за один раз, понад 10 000 одержувачів на день або понад 30 повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="5d7f9-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="5d7f9-108">Під час запуску робочого циклу повідомлення електронної пошти не надсилається, і ви помітите таку поведінку:</span><span class="sxs-lookup"><span data-stu-id="5d7f9-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="5d7f9-109">Для робочого циклу за допомогою типу платформи SharePoint 2013 можна перейти на сторінку " **стан робочого циклу** ".</span><span class="sxs-lookup"><span data-stu-id="5d7f9-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="5d7f9-110">На сторінці "стан робочого циклу" установлено **внутрішній стан** " **початок**", а повітряна кулька "відомості" **не може бути надіслано одержувачу**.</span><span class="sxs-lookup"><span data-stu-id="5d7f9-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="5d7f9-111">Щоб вирішити цю проблему, настройте робочий цикл, щоб надсилати повідомлення електронної пошти, не перевищивши [обмеження відправника Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="5d7f9-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="5d7f9-112">Наприклад, за допомогою паузи в робочому циклі надішліть повідомлення електронної пошти до групи Microsoft 365, групі розсилки або з увімкнутою безпекою пошти або надішліть повідомлення менше, ніж 200 одержувачам за один раз.</span><span class="sxs-lookup"><span data-stu-id="5d7f9-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="5d7f9-113">Щоб отримати докладніші відомості, ознайомтеся з наведена нижче [статтею](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="5d7f9-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="5d7f9-114">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="5d7f9-114">Related topics</span></span>
- [<span data-ttu-id="5d7f9-115">Створення потоку</span><span class="sxs-lookup"><span data-stu-id="5d7f9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5d7f9-116">SharePoint і передавання</span><span class="sxs-lookup"><span data-stu-id="5d7f9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 