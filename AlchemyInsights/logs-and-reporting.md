---
title: Журнали та звіти
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036101"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="6bde2-102">Журнали та звіти</span><span class="sxs-lookup"><span data-stu-id="6bde2-102">Logs and Reporting</span></span>

<span data-ttu-id="6bde2-103">Запитання й відповіді про повідомлення про те, як повідомити про Azure [Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) (AZURE AD), які часто задаються.</span><span class="sxs-lookup"><span data-stu-id="6bde2-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="6bde2-104">Докладні відомості наведено в статті створення [звіту про службу "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)".</span><span class="sxs-lookup"><span data-stu-id="6bde2-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="6bde2-105">**Вирішення проблем із аудитом**</span><span class="sxs-lookup"><span data-stu-id="6bde2-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="6bde2-106">Якщо у вас виникли проблеми з деякими аудиторською діяльністю, а в цьому [списку](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)відсутня робота, введіть квиток підтримки.</span><span class="sxs-lookup"><span data-stu-id="6bde2-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="6bde2-107">Якщо у вас виникли проблеми з відображенням будь-яких журналів аудиту в клієнті, надішліть квиток на службу підтримки.</span><span class="sxs-lookup"><span data-stu-id="6bde2-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="6bde2-108">Якщо ваші аудиторські дії не відображаються безпосередньо на порталі Лазурне, ознайомтеся з нашою [інформацією про латентність](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) та File квитків служби підтримки, якщо затримка перевищує документовану затримку.</span><span class="sxs-lookup"><span data-stu-id="6bde2-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="6bde2-109">Збереження журналів дій у Лазур</span><span class="sxs-lookup"><span data-stu-id="6bde2-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="6bde2-110">Якщо ви не бачите всі елементи аудиту для вибраного діапазону дат, ви можете завантажити до рядків на 250K (за останнім часом) для входу на порталі Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="6bde2-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="6bde2-111">Докладні відомості наведено в статті [завантаження дій з аудиту](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="6bde2-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="6bde2-112">**Вирішення проблем із входом**</span><span class="sxs-lookup"><span data-stu-id="6bde2-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="6bde2-113">Ви можете переглянути останні 30 днів даних, якщо у вас є ліцензія Azure AD Premium (P1 або P2) для вашого клієнта.</span><span class="sxs-lookup"><span data-stu-id="6bde2-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="6bde2-114">Для входу доступні лише для орендарів Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="6bde2-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="6bde2-115">Він недоступний для безкоштовних і основних ліцензованих орендарів.</span><span class="sxs-lookup"><span data-stu-id="6bde2-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="6bde2-116">Якщо ваш клієнт має ліцензію Premium P1, і ви не бачите їх, ознайомтеся з [відомостями про затримку](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) та файлами служби підтримки, якщо затримка перевищує документовану затримку.</span><span class="sxs-lookup"><span data-stu-id="6bde2-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="6bde2-117">Якщо ви не бачите всі елементи входу для вибраного діапазону дат, зверніть увагу, що ви можете завантажити до рядків на 250K (за останнім часом) для входу з порталу Лазур.</span><span class="sxs-lookup"><span data-stu-id="6bde2-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="6bde2-118">Додаткові відомості наведено в статті [завантаження дій для входу](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="6bde2-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="6bde2-119">**Виправлення неполадок із звітами про безпеку (користувачі, позначені під загрозою ризику, ризиковане вхід)**</span><span class="sxs-lookup"><span data-stu-id="6bde2-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="6bde2-120">Користувачі, позначені для звіту про безпеку ризику</span><span class="sxs-lookup"><span data-stu-id="6bde2-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="6bde2-121">Ризикований звіт про вхід на порталі «блакитний каталог Active Directory»</span><span class="sxs-lookup"><span data-stu-id="6bde2-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="6bde2-122">Події ризику в службі "блакитні активні каталоги"</span><span class="sxs-lookup"><span data-stu-id="6bde2-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
