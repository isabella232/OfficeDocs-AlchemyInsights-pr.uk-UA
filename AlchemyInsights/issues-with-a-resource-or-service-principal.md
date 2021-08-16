---
title: Проблеми з ресурсом або основним ім'ям служби
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028097"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Проблеми з ресурсом або основним ім'ям служби

1. Якщо ви лише починаєте роботу, об'єкти-учасники програм і служб [у Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) описують реєстрацію програм, об'єкти програм і принципи служби в Azure Active Directory: що вони є, як вони використовуються та як вони пов'язані між собою. Приклад сценарію для кількох клієнтів також проілюстровано зв'язок між об'єктом програми програми та відповідними основними об'єктами служби.
2. Щоб дізнатися більше про зв'язки між програмами та основними учасниками служби, прочитайте програми та об'єкти основної служби [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. Інструкції. На порталі можна створити програму й основне ім'я служби [Azure AD,](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) до яких можна отримати доступ до ресурсів, і показано, як створити нову програму та основне ім'я служби Azure Active Directory (Azure AD), яку можна використовувати з елементом керування доступом на основі ролей.
4. За [допомогою основного API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)служби можна програмно керувати екземплярами програм і керувати функціями програми у вашому клієнта.
5. [тип ресурсу "віндципальна](https://docs.microsoft.com/graph/api/resources/serviceprincipal) служба" – це список усіх властивостей і методів для типу ресурсу "Principal" у службі.
6. [Відмінності між типами ресурсів Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) відмінності між Azure AD Graph і Microsoft Graph ресурсів. У ньому відображаються ресурси з різними іменами або недоступні; Тут також виділено ресурси, доступні в бета-версії Microsoft Graph але не доступні у версії 1.0.

**Проблеми з користувачами-гостів**

- [Короткий посібник.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Додавання користувачів-гостей до каталогу на порталі Azure показує, як додати нового гостя до каталогу Azure AD через портал Azure, надіслати запрошення та дізнатися, як виглядає процес використання запрошення гостя.
- [Навчальна вправа.](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) Створюйте потоки користувачів Azure Active Directory B2C покаже, як створити кілька рекомендованих потоків користувачів на порталі Azure. Відомості про те, як налаштувати потік паролів власників ресурсів (ROPC) у програмі, див. в статті Налаштування облікових даних власника ресурсів в Azure AD B2C.
