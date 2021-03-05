---
title: Настроювання служби надання послуг
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484048"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="9114d-102">Настроювання служби надання послуг</span><span class="sxs-lookup"><span data-stu-id="9114d-102">Configuring the Provision service</span></span>

<span data-ttu-id="9114d-103">Для автоматичного підготовки користувача до роботи, Azure AD потребує припустимих облікових даних, які дають змогу підключитися до API веб-служб робочого дня.</span><span class="sxs-lookup"><span data-stu-id="9114d-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="9114d-104">Крім того, кнопка "тестовий зв'язок" в програмі "робочий день" для підготовки користувачів AD також перевіряє, чи можна підключитися до агента підготовки з використанням служби Azure AD Connect, пов'язаного з доменом AD.</span><span class="sxs-lookup"><span data-stu-id="9114d-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="9114d-105">Якщо на порталі Лазурне з'являється повідомлення про помилку під час збереження облікових даних, виконайте Рекомендовані дії нижче.</span><span class="sxs-lookup"><span data-stu-id="9114d-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="9114d-106">Переконайтеся, що ви налаштували обліковий запис користувача системи інтеграції в день, як зазначено в розділі навчальний розділ [Настроювання користувача системи інтеграції в будні](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)дні.</span><span class="sxs-lookup"><span data-stu-id="9114d-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="9114d-107">Переконайтеся, що служба агента підготовки Azure AD Connect працює на локальному сервері Windows за допомогою консолі керування службами.</span><span class="sxs-lookup"><span data-stu-id="9114d-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="9114d-108">Ви також можете перевірити стан агента на Лазуропорталі, натиснувши кнопку Переглянути локальні агенти.</span><span class="sxs-lookup"><span data-stu-id="9114d-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="9114d-109">Переконайтеся, що ви вводите значення в полі "ім'я користувача для робочого дня" за допомогою формату username@workday-клієнта – імені клієнта.</span><span class="sxs-lookup"><span data-stu-id="9114d-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="9114d-110">Якщо робочий день – ім'я клієнта відсутнє, автентифікація робочого дня не виконується.</span><span class="sxs-lookup"><span data-stu-id="9114d-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="9114d-111">Якщо ви настроюючи інтеграцію з клієнтом реалізації робочого дня, зверніть увагу на час запланованого простоїв вашого клієнта робочого дня.</span><span class="sxs-lookup"><span data-stu-id="9114d-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="9114d-112">Робочий день запланував час для його реалізації для орендарів у вихідні дні (зазвичай з п'ятниці увечері до суботи) і збої підключення під час цього вікна простоїв є відомою проблемою, яку автоматично вирішує, як тільки для того, щоб мешканці, що здійснюються, знову в онлайні.</span><span class="sxs-lookup"><span data-stu-id="9114d-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="9114d-113">Інколи може з'явитися таке повідомлення про помилку, якщо ви змінили пароль користувача системи інтеграції через оновлення клієнта або якщо обліковий запис заблоковано або завершився.</span><span class="sxs-lookup"><span data-stu-id="9114d-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="9114d-114">Перевірте стан користувача системи інтеграції з адміністратором робочого дня.</span><span class="sxs-lookup"><span data-stu-id="9114d-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="9114d-115">Докладні відомості про настроювання робочого дня для автоматизованого підготовки наведено в статті [навчальний посібник: Настроювання робочого дня для автоматичного підготовки користувача](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="9114d-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
