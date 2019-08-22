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
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539050"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="f706f-102">Визначити IP-адресу та клієнта в журнали аудиту</span><span class="sxs-lookup"><span data-stu-id="f706f-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="f706f-103">IP-адресу, яка відповідає активності користувача Office 365 або адміністратор показано журнали аудиту.</span><span class="sxs-lookup"><span data-stu-id="f706f-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="f706f-104">Інформація клієнта також записується.</span><span class="sxs-lookup"><span data-stu-id="f706f-104">The client information is also logged.</span></span> <span data-ttu-id="f706f-105">Ось кроки для виявлення такої інформації</span><span class="sxs-lookup"><span data-stu-id="f706f-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="f706f-106">Увійдіть до [Office 365 безпеки & центрі дотримання](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f706f-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f706f-107">Перейти до **пошуку** > сторінку**пошуку журналу аудиту** .</span><span class="sxs-lookup"><span data-stu-id="f706f-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="f706f-108">Якщо ви зацікавлені в певної дії, виберіть його зі списку **діяльності** .</span><span class="sxs-lookup"><span data-stu-id="f706f-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="f706f-109">Якщо ні, то буде повернуто всі заходи для вибраного користувача (за замовчуванням).</span><span class="sxs-lookup"><span data-stu-id="f706f-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="f706f-110">**Примітка**: певні заходи можуть бути недоступними в меню **діяльності** ; Тим не менш, ті аудиту елементи будуть повернуті, якщо **Показати результати для всіх видів діяльності** є виділеного (налаштування за умовчанням).</span><span class="sxs-lookup"><span data-stu-id="f706f-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="f706f-111">Вказати ім'я користувача в полі **користувачі** , виберіть відповідний проміжок часу для активності і натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="f706f-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="f706f-112">В результатах пошуку ви можете побачити IP-адресу для що діяльність в області результатів.</span><span class="sxs-lookup"><span data-stu-id="f706f-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="f706f-113">Виберіть запис аудиту, щоб побачити детальну інформацію в спливаюче **деталі** (наприклад, клієнт, користувач, який виконано дію, і т. д.).</span><span class="sxs-lookup"><span data-stu-id="f706f-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="f706f-114">Докладніше перегляньте статтю [знайти IP-адресу комп'ютера, який використовується для доступу до порушення безпеки облікового запису](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="f706f-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
