---
title: 'AIP: політики поведінки не так, як очікувалося'
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821648"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: політики поведінки не так, як очікувалося

Захист даних в Azure. Політики, які не поводяться належним чином, див. в наведених нижче рекомендаціях щодо різних проблем політики.

1. Якщо у вас виникають проблеми з візуальною маркуванням, перевірте, коли застосовуються [візуальні позначення.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Якщо виникають проблеми з автоматичним підписуванням, ознайомтеся зі статтями Як [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)налаштувати умови для автоматичної та рекомендованої класифікації для захисту даних [в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) і Який вигляд мають типи відомостей.
3. Якщо у вас виникають проблеми з захистом власного файлу або Pfile, перегляньте [конфігурацію файлу API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Перевірте, чи використовується ненастроєні вами масштабовані політики: Налаштування політики захисту даних Azure для певних користувачів за допомогою масштабних [політик.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Якщо автоматичне маркування не працює в Outlook під час вкладення документа з підписами, переконайтеся, що DRMEncryptProperty не визначено, як описано в статті Параметри реєстру [IRM для](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)безпеки.

Якщо проблеми не зникають, збирайте журнали клієнта Azure Information Protection і вкладіть експортовані журнали до цього запиту.

1. Відкрийте документ Office або створіть електронний лист у програмі Outlook.
2. Натисніть **кнопку Довідка та відгуки щодо** захисту та  >  **чутливості.**
3. Натисніть **кнопку Експорт журналів**.
4. Збережіть журнали у вибраному розташуванні та вкладіть їх до цього запиту на обслуговування.

Додаткові ресурси:

- [Налаштування мітки для візуальних позначок для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Перегляд документації для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Використання міток чутливості в програмах Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

