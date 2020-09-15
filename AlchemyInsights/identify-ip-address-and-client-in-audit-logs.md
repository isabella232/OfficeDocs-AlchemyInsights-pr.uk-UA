---
title: Визначення IP-адреси та клієнта в журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668331"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="504fe-102">Визначення IP-адреси та клієнта в журналах аудиту</span><span class="sxs-lookup"><span data-stu-id="504fe-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="504fe-103">IP-адреса, що відповідає діяльності користувача або адміністратора Microsoft 365, відображається в журналах аудиту.</span><span class="sxs-lookup"><span data-stu-id="504fe-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="504fe-104">Відомості про клієнта також записуються.</span><span class="sxs-lookup"><span data-stu-id="504fe-104">The client information is also logged.</span></span> <span data-ttu-id="504fe-105">Нижче наведено інструкції з виявлення такої інформації.</span><span class="sxs-lookup"><span data-stu-id="504fe-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="504fe-106">Увійдіть у [центр відповідності & безпеки Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="504fe-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="504fe-107">Перейдіть на сторінку **Search**  >  **Пошук журналу аудиту** .</span><span class="sxs-lookup"><span data-stu-id="504fe-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="504fe-108">Якщо вас цікавить певна дія, виберіть його зі списку **дії** .</span><span class="sxs-lookup"><span data-stu-id="504fe-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="504fe-109">Якщо ні, усі дії будуть повернуті для вибраного користувача (настройки за замовчуванням).</span><span class="sxs-lookup"><span data-stu-id="504fe-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="504fe-110">**Примітка**. деякі дії можуть бути недоступні в меню " **дії** ". Проте ці елементи аудиту буде повернуто, якщо вибрано параметр **Відображати результати для всіх дій** (Настроювання за замовчуванням).</span><span class="sxs-lookup"><span data-stu-id="504fe-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="504fe-111">Укажіть ім'я користувача в полі **користувачі** , виберіть відповідний діапазон дат для дії, а потім натисніть кнопку **Search (пошук**).</span><span class="sxs-lookup"><span data-stu-id="504fe-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="504fe-112">У результатах можна переглянути IP-адресу для цієї дії в області результатів.</span><span class="sxs-lookup"><span data-stu-id="504fe-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="504fe-113">Виберіть запис аудиту, щоб переглянути докладні відомості в надбудові " **відомості** " (наприклад, клієнт, користувач, який виконав дію тощо).</span><span class="sxs-lookup"><span data-stu-id="504fe-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="504fe-114">Докладні відомості наведено в статті [Пошук IP-адреси комп'ютера, який використовується для доступу до скомпрометований обліковий запис](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="504fe-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
