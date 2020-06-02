---
title: 'AIP: політики, не поведінки належним чином'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506579"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: політики, не поведінки належним чином

Відомості про захист Azure: політики не поводяться належним чином, перегляньте наведені нижче рекомендації щодо рекомендацій щодо різних питань політики:

1. Якщо у вас виникли проблеми з візуальними відмітками, будь ласка, перегляньте, [коли застосовуються візуальні позначки](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Якщо у вас виникли проблеми з автоматичним етикеткуванням, будь ласка, перегляньте, [як налаштувати умови для автоматичної та рекомендованою класифікації для захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) та для [яких типів конфіденційних даних шукати](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Якщо у вас виникли проблеми з рідним/Pfile захист, будь ласка, перевірте [Конфігурація файлу API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Перевірте, якщо використовуються політики в області, які не настроєно належним чином: [Настроювання політики захисту даних Azure для певних користувачів за допомогою політики в](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)області.
5. Якщо автоматичне позначення не працює для Outlook під час підключення документа з міткою, переконайтеся, що DRMEncryptProperty не визначено, як описано тут: [Параметри реєстру IRM для безпеки](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Якщо ви все ще зіткнулися з проблемами, будь ласка, збирайте журнали клієнт захисту інформації Azure і Прикріпіть експортовані журнали до цього квитка.

1. Відкрийте документ Office або створіть новий електронний лист у програмі Outlook.
2. Натисніть кнопку **захист/чутливість**  >  **Довідка та зворотній зв'язок**.
3. Натисніть кнопку **експортувати журнали**.
4. Збережіть журнали на ваш вибір місця розташування та Прикріпіть їх до цього запиту послуги.

Додаткові ресурси:

- [Настроювання Мітки для візуального розмітки для захисту інформації в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Огляд документації з захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Використання міток чутливості у програмах Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

