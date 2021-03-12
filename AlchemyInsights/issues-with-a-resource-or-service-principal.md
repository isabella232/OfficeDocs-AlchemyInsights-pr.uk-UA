---
title: Проблеми з основним ресурсом або службою
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714464"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Проблеми з основним ресурсом або службою

1. Якщо ви тільки починаєте роботу, [програми та служби основних об'єктів у Лазурому Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) , описано, як реєстрація програм, об'єкти застосунків і керівники служб у службі Azure Active Directory: що вони є, як вони використовуються, і як вони пов'язані між собою. Також пропонується приклад сценарію багатоклієнтської роботи, щоб проілюструвати зв'язок між об'єктом застосунку програми та відповідними основними об'єктами служби.
2. Ви можете дізнатися більше про зв'язок між програмами та службами, читаючи [програми та основні об'єкти в області Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Як використовувати портал для створення поштової програми та основної служби AD, які можуть отримати доступ до ресурсів](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) , у цій статті описано, як створити нову службу "Лазурний" (AZURE AD), яку можна використовувати для керування доступом на основі ролей.
4. Використовуючи [основний API служби](https://docs.microsoft.com/graph/api/resources/serviceprincipal), можна програмно керувати екземплярами програм і керувати тим, що може виконувати програма в клієнті.
5. [тип ресурсу servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) містить перелік усіх властивостей і методів для типу ресурсів servicePrincipal.
6. [Відмінності між типами ресурсів у AZURE AD Graph і Microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) Graph відрізняються між відмінностями в лазуровий рекламний граф і ресурсами Microsoft графа. У ньому відображаються ресурси, які містять різні імена або недоступні; Вона також виділяє ресурси, доступні в бета-версії Microsoft Graph, але не у версії v 1.0.

**Проблеми з гостьовими користувачами**

- [QuickStart: додавання користувачів-гостей до каталогу на порталі «Лазурний](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) » показує, як додати нового гостя користувача до свого лазуроподібного каталогу за допомогою порталу "Лазурний", надіслати запрошення та дізнатися, як виглядатиме процес викупу запрошення гостей гостьового користувача.
- [Навчальний посібник: створення потоків користувачів у B2C у службі Azure Active Directory](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) показує, як створити Рекомендовані потоки користувачів за допомогою порталу "Лазурний". Якщо ви шукаєте відомості про те, як настроїти потік облікових даних паролів ресурсу (РОПК) у програмі, ознайомтеся з настроюванням передавання облікових даних власника ресурсу в Azure AD B2C.
