---
title: 'AIP: політики, які не ведуть себе належним чином'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663210"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: політики, які не ведуть себе належним чином

Azure захисту інформації: політики не ведуть себе належним чином, ознайомтеся з такими порадами щодо рекомендованих рекомендацій для різних питань політики.

1. Якщо у вас виникли проблеми з візуальним розміткою, перевірте, [чи застосовуються візуальні позначки](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Якщо у вас виникли проблеми з автоматичним етикетуванням, ознайомтеся з тим, [як настроїти умови для автоматичної та рекомендованої класифікації для служби Azure захисту інформації](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) , а [також про те, які типи конфіденційної інформації шукають](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Якщо у вас виникли проблеми зі службою захисту від рідної та Pfile, перегляньте [КОНФІГУРАЦІЮ API для файлів](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Перевірте, чи ви використовуєте політики, які не настроєно належним чином: [як настроїти політику захисту інформації в Лазур для певних користувачів за допомогою політик рівня](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Якщо автоматичне маркування не працює в Outlook під час приєднання до документа з позначкою, переконайтеся, що DRMEncryptProperty не визначено, як описано тут: [Параметри реєстру IRM для системи безпеки](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Якщо у вас все ще виникають проблеми, Зберіть клієнт для захисту інформації з Azure, а також вкладіть експортовані журнали до цього квитка.

1. Відкрийте документ Office або створіть новий електронний лист у програмі Outlook.
2. Виберіть посилання **захист/конфіденційність**  >  **і зворотний зв'язок**.
3. Натисніть кнопку **експорт журналів**.
4. Збережіть журнали на своєму виборі розташування та вкладіть їх до цього запиту на обслуговування.

Додаткові ресурси:

- [Настроювання підпису для візуального маркування для захисту інформації за допомогою Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Огляд документації з захисту інформації про Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Використання міток чутливості у програмах Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

