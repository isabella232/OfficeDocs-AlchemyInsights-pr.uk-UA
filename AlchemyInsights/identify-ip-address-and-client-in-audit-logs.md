---
title: Визначення IP-адресу та клієнта в журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716409"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="9365e-102">Визначення IP-адресу та клієнта в журналах аудиту</span><span class="sxs-lookup"><span data-stu-id="9365e-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="9365e-103">IP-адресу, яка відповідає діяльності користувача або адміністратора Microsoft 365 відображається в журналах аудиту.</span><span class="sxs-lookup"><span data-stu-id="9365e-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="9365e-104">Інформація про клієнта також реєструється.</span><span class="sxs-lookup"><span data-stu-id="9365e-104">The client information is also logged.</span></span> <span data-ttu-id="9365e-105">Ось кроки для ідентифікації такої інформації</span><span class="sxs-lookup"><span data-stu-id="9365e-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="9365e-106">Увійдіть до [Microsoft 365 безпеки & центр відповідності](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9365e-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9365e-107">Перейдіть на сторінку **Search** > **пошуку журналу аудиту** пошуку.</span><span class="sxs-lookup"><span data-stu-id="9365e-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="9365e-108">Якщо ви зацікавлені в певній діяльності, виберіть її зі списку **справ** .</span><span class="sxs-lookup"><span data-stu-id="9365e-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="9365e-109">Якщо ні, усі справи буде повернуто вибраному користувачу (параметр за промовчанням).</span><span class="sxs-lookup"><span data-stu-id="9365e-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="9365e-110">**Примітка**: певні дії можуть бути недоступними в меню **дії** ; Проте ці елементи аудиту буде повернуто, якщо вибрано **відображення результатів для всіх дій** (параметр за промовчанням).</span><span class="sxs-lookup"><span data-stu-id="9365e-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="9365e-111">Вкажіть ім'я користувача в полі **користувачі** , виберіть відповідний діапазон дат для справи, а потім натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="9365e-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="9365e-112">У результатах пошуку можна побачити IP-адресу для цієї справи в області результатів.</span><span class="sxs-lookup"><span data-stu-id="9365e-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="9365e-113">Виберіть запис аудиту, щоб переглянути докладні відомості в спливаючому меню **подробиць** (наприклад, клієнт, користувач, який виконував дії тощо).</span><span class="sxs-lookup"><span data-stu-id="9365e-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="9365e-114">Для отримання додаткових відомостей див. [Пошук IP-адреси комп'ютера, що використовується для доступу до скомпрометований обліковий запис](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="9365e-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
