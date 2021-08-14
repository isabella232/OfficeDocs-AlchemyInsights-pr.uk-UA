---
title: 'AIP: колонтитули не відображаються належним чином'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: e3a0e5caccba87ddd8e4c786b5c8918494e709b6f4d5d60e7c31215a60b1d5d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951802"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: колонтитули не відображаються належним чином

Якщо виникають проблеми з візуальним позначенням, які не відображаються належним чином, перегляньте наведені нижче рекомендації.

1. Переконайтеся, що ви перевірили, [коли застосовано візуальні позначення.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Щоб Office, ознайомтеся з датою, [Office 365 застосовує позначення вмісту та шифрування.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)
3. Якщо потрібно видалити наявні колонтитули, ознайомтеся зі стосом Видалення колонтитулів з інших рішень [для підписування.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)

Якщо проблема не зникає, збирайте журнали клієнта Захисту даних Azure і вкладіть експортовані журнали до цього запиту.

**Експорт журналів захисту даних в Azure**

1. Відкрийте документ Office або створіть електронний лист у Outlook.
2. Натисніть **кнопку Довідка та відгуки щодо** захисту та  >  **чутливості.**
3. Натисніть **кнопку Експорт журналів**.
4. Збережіть журнали у вибраному розташуванні та вкладіть їх до цього запиту на обслуговування.

Докладні відомості див. в такому:

- [Налаштування мітки для візуальних позначок для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Перегляд документації для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Вимоги до захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Короткий посібник із захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Завантаження клієнта Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
