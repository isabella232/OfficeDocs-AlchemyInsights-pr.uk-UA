---
title: Автоматична класифікація не працює належним чином за допомогою клієнта AIP
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979730"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Автоматична класифікація не працює належним чином за допомогою клієнта AIP

Автоматична класифікація не працює належним чином, використовуйте наведені нижче рекомендовані рекомендації.

1. Якщо виникають проблеми з автоматичним підписуванням, див. статті Як налаштувати [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)умови для автоматичної та рекомендованої класифікації для захисту даних [в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) і Який вигляд мають типи відомостей.
2. Перевірте, чи використовується ненастроєні вами масштабовані політики: Налаштування політики захисту даних Azure для певних користувачів за допомогою масштабних [політик.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Якщо автоматичне маркування не працює в Outlook під час вкладення документа з підписом, переконайтеся, що параметри реєстру IRM для безпеки не `DRMEncryptProperty` [визначено нижче.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Якщо ви використовували [вбудовані типи даних](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) для політики захисту даних Azure, переконайтеся, що вміст відповідає очікуваному форматі.
5. Переконайтеся, що етикетку настроєно на значення Автоматично **або** **Рекомендоване**. (**Автоматичне** маркування доступне для всіх програм  Microsoft 365, а рекомендується для всіх програм Microsoft 365, крім Outlook).)
6. Автоматичну класифікацію не можна використовувати для документів і повідомлень електронної пошти, які раніше були автоматично позначені або автоматично позначені вищою класифікацією.  Докладні відомості див. в статті [Застосування автоматичних або рекомендованих етикеток.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Якщо проблеми не зникають, зберіть журнали клієнта Azure Information Protection і вкладіть експортовані журнали до запиту на підтримку. Щоб експортувати журнали захисту даних в Azure:
    - Відкрийте документ Office або створіть електронний лист у Outlook.
    - Натисніть **кнопку Довідка та відгуки щодо** захисту та  >  **чутливості.**
    - Натисніть **кнопку Експорт журналів**.
    - Збережіть журнали у вибраному розташуванні та вкладіть їх у свій запит на обслуговування.

Докладні відомості див. в такому:

- [Налаштування умов для автоматичної та рекомендованої класифікації для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Інструкції для типових сценаріїв, у яких використовується захист даних в Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Перегляд документації для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Перегляд передплат і функцій для захисту даних в Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Вимоги до захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Короткий посібник із захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Завантаження клієнта Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
