---
title: Автоматична класифікація не поводиться належним чином з клієнтом AIP
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508397"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Автоматична класифікація не поводиться належним чином з клієнтом AIP

Автоматична класифікація не поводиться належним чином, скористайтеся такими рекомендованими рекомендаціями:

1. Якщо у вас виникли проблеми з автоматичним етикеткуванням, Дізнайтеся, [як налаштувати умови для автоматичної та рекомендованою класифікації для захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) та [для яких типів конфіденційних даних шукати](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Перевірте, якщо використовуються політики в області, які не настроєно належним чином: [Настроювання політики захисту даних Azure для певних користувачів за допомогою політики в](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)області.
3. Якщо автоматичне позначення не працює для Outlook під час підключення документа з міткою, переконайтеся, що `DRMEncryptProperty` не визначено, як описано тут: [Параметри реєстру IRM для безпеки](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Якщо ви використали [вбудовані типи інформації](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) для вашої політики захисту інформації в Azure, перевірте, чи відповідає ваш вміст очікуваним форматом.
5. Переконайтеся, що підпис належним чином налаштовано на **Автоматичне** або **рекомендоване**. (**Автоматичне** маркування доступне для всіх програм Office, тоді як **рекомендовано** доступно для всіх програм Office, крім Outlook.)
6. Автоматичну класифікацію для документів і електронних листів, раніше позначених вручну або раніше автоматично позначені з вищою класифікацією, використовувати не можна.  Для отримання додаткових відомостей див.: [як застосовуються автоматичні або Рекомендовані Мітки](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Якщо ви все ще зіткнулися з проблемами, будь ласка, збирайте журнали клієнт захисту інформації Azure і Прикріпіть експортовані журнали до квитка підтримки. Щоб експортувати журнали захисту інформації в Azure:
    - Відкрийте документ Office або створіть новий електронний лист у програмі Outlook.
    - Натисніть кнопку **захист/чутливість**  >  **Довідка та зворотній зв'язок**.
    - Натисніть кнопку **експортувати журнали**.
    - Збережіть журнали на вибір місцеположення та Прикріпіть їх до вашого запиту на обслуговування.

За додатковою інформацією див.:

- [Настроювання умов для автоматичної та рекомендованою класифікації для захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Інструкції для поширених сценаріїв, які використовують Azure захисту інформації](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Огляд документації з захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Огляд підписок та функцій захисту інформації Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Вимоги для захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Короткий посібник з захисту інформації для Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Завантажити клієнт для захисту інформації Azure](https://www.microsoft.com/download/details.aspx?id=53018)
