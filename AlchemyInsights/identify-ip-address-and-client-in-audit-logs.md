---
title: Визначити IP-адресу та клієнта в журнали аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382974"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="5edc8-102">Визначити IP-адресу та клієнта в журнали аудиту</span><span class="sxs-lookup"><span data-stu-id="5edc8-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="5edc8-103">IP-адресу, яка відповідає діяльності користувач або адміністратор показано журнали аудиту.</span><span class="sxs-lookup"><span data-stu-id="5edc8-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="5edc8-104">Інформація клієнта також записується.</span><span class="sxs-lookup"><span data-stu-id="5edc8-104">The client information is also logged.</span></span> <span data-ttu-id="5edc8-105">Ось кроки для виявлення такої інформації</span><span class="sxs-lookup"><span data-stu-id="5edc8-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="5edc8-106">Увійдіть до [Office 365 безпеки & відповідно центр](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="5edc8-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="5edc8-107">Натисніть кнопку **Пошук та розслідування** та виберіть **Пошук журналу аудиту**.</span><span class="sxs-lookup"><span data-stu-id="5edc8-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="5edc8-108">Якщо ви зацікавлені в певної дії, виберіть його зі списку **діяльності** .</span><span class="sxs-lookup"><span data-stu-id="5edc8-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="5edc8-109">Якщо ні, то буде повернуто всі заходи для вибраного користувача (за замовчуванням).</span><span class="sxs-lookup"><span data-stu-id="5edc8-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="5edc8-110">**Примітка**: певні заходи можуть бути недоступними в меню **діяльності** ; Тим не менш, ті аудиту елементи будуть повернуті, якщо **Показати результати для всіх видів діяльності** є виділеного (налаштування за умовчанням).</span><span class="sxs-lookup"><span data-stu-id="5edc8-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="5edc8-111">Вказати ім'я користувача в полі **користувачі** , виберіть відповідний проміжок часу для активності і натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="5edc8-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="5edc8-112">В результатах пошуку ви можете побачити IP-адресу для що діяльність в області результатів.</span><span class="sxs-lookup"><span data-stu-id="5edc8-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="5edc8-113">Виберіть запис аудиту, щоб побачити детальну інформацію в спливаюче **деталі** (наприклад, клієнт, користувач, який виконано дію, і т. д.).</span><span class="sxs-lookup"><span data-stu-id="5edc8-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="5edc8-114">Докладніше перегляньте статтю [знайти IP-адресу комп'ютера, який використовується для доступу до порушення безпеки облікового запису](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="5edc8-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
