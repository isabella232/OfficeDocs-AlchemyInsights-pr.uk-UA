---
title: Проблема з окремим користувачем
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430357"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="89d36-102">Проблема з окремим користувачем</span><span class="sxs-lookup"><span data-stu-id="89d36-102">Problem with single user</span></span>

- <span data-ttu-id="89d36-103">Можливо, користувача не підготовлено, тому що служба ще не має можливості оцінити користувача.</span><span class="sxs-lookup"><span data-stu-id="89d36-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="89d36-104">Перегляньте вказівки про те, як довго триває підготовка, а також рядок перебігу на сторінці конфігурації підготовки.</span><span class="sxs-lookup"><span data-stu-id="89d36-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="89d36-105">Якщо в розділі Додаткові відомості вказано стійкий стан до дати, коли користувач створив або оновив або видалив, це означає, що ви ще не встигли оцінити користувача.</span><span class="sxs-lookup"><span data-stu-id="89d36-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="89d36-106">У цьому випадку найкраще чекати, доки служба підготовки завершиться.</span><span class="sxs-lookup"><span data-stu-id="89d36-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="89d36-107">Зверніть увагу, що наша служба знає лише зміни, внесені користувачем у вихідній системі (хмарний HR).</span><span class="sxs-lookup"><span data-stu-id="89d36-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="89d36-108">Для визначення змін і передавання її у службу Active Directory має бути припустиме змінення вихідної системи для Azure AD.</span><span class="sxs-lookup"><span data-stu-id="89d36-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="89d36-109">Служба підготовки оцінювала користувача та визначає, що його не можна підготувати:</span><span class="sxs-lookup"><span data-stu-id="89d36-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="89d36-110">Якщо ви встановили атрибут, оснований на основі фільтра, переконайтеся, що користувач відповідає вказаним умовам.</span><span class="sxs-lookup"><span data-stu-id="89d36-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="89d36-111">Якщо користувачі вже існують в цільовій системі та стан користувача у вихідному та цільовому збігу, ми не будемо виконувати подальші дії.</span><span class="sxs-lookup"><span data-stu-id="89d36-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="89d36-112">Служба підготовки спробувала підготувати користувача та не зміг його виконати.</span><span class="sxs-lookup"><span data-stu-id="89d36-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="89d36-113">Для цих сценаріїв перегляньте вкладку виправлення неполадок і рекомендацій для журналів підготовки:</span><span class="sxs-lookup"><span data-stu-id="89d36-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="89d36-114">Обов'язковий атрибут для користувача, можливо, відсутній у локальній службі Active Directory або в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="89d36-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="89d36-115">Наприклад, правила покоління userPrincipalName або sAMAccountName не генерують потрібне значення.</span><span class="sxs-lookup"><span data-stu-id="89d36-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="89d36-116">Атрибут відповідного атрибута (зазвичай employeeId) не розв'яже унікальний користувач у локальній службі Active Directory або Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="89d36-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="89d36-117">Наприклад, існує два користувачі з тим самим employeeId в ОГОЛОШЕННІ, а служба повертає код помилки, щоб позначити повторювані записи призначення для одного запису.</span><span class="sxs-lookup"><span data-stu-id="89d36-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="89d36-118">Щоб переглянути журнали для окремих користувачів і груп, ознайомтеся [зі статтею перегляд журналів підготовки для певної проблеми з певним користувачем](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="89d36-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
