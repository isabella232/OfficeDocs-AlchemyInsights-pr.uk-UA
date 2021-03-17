---
title: Настроювання єдиного входу (SSO)
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841668"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Настроювання єдиного входу (SSO)

**Настроювання програм**

1. Ви повинні отримати значення з постачальника програм. Ви можете вручну вказати значення або передати файл метаданих, щоб витягти значення полів.
2. Багато програм уже настроєно для роботи з Azure AD. Ці програми наведено в колекції програм, які можна переглядати, коли ви додаєте програму до свого клієнта Azure AD. [Цикл швидкого запуску](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) проходить процес.
3. Щоб створити програму, яка не є колекцією, можна натиснути кнопку **+ створити власну програму** та надати ім'я для своєї програми.
    - За замовчуванням буде вибрано **інтегрувати будь-яку іншу програму, яку не можна виявити в колекції** , яка є правильним варіантом для програм, які не використовують галерею.
    - Після натискання кнопки " **створити** " після введення імені для програми буде створено нову програму, яка не є колекцією для підприємств.
    - Після цього ви можете переходити на **єдиний вхід** у розділі **керування** цією програмою, і ви зможете переглянути різні методики для її реалізації у вашому середовищі.

**Настроювання безшовного єдиного входу для певної програми**

Для програм у колекції ви зможете знайти докладні покрокові вказівки. Щоб отримати доступ до цих кроків, ви можете переглянути список усіх підручників із конфігурації програм [SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Настроювання єдиного входу на основі SAML**

1. [QuickStart: налаштування єдиного входу (SSO) для програми в клієнті Azure Active Directory (Лазурний рекламний)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Щоб дізнатися більше про параметр "на основі SAML" для служби "єдиний вхід", ознайомтеся з відомостями про службу " [єдиний вхід" на основі SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Щоб дізнатися про запити автентифікації SAML 2,0 і відповідей, які підтримує "Лазурний" (Azure AD), підтримуються для єдиного Sign-On (SSO), ознайомтеся з [єдиним Sign-On SAML-протоколом](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Щоб дізнатися, як створити та настроїти єдиний вхід на основі SAML (SSO) для програми в Лазурому Active Directory (Azure AD) за допомогою API Microsoft Graph, перегляньте статтю [настроїти єдиний вхід на основі SAML для своєї програми за допомогою API Microsoft Graph](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Щоб дізнатися, як Azure AD використовує протокол SAML, Дізнайтеся, [як платформа ідентифікації Microsoft використовує протокол SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Настроювання маркерів і тверджень**

1. [Як настроїти претензії, видані в маркер SAML для корпоративних програм](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Щоб дізнатися, як настроїти претензії за допомогою PowerShell, Дізнайтеся, [як настроїти претензії, що випускаються в маркерів для певної програми в клієнті (ознайомлювальну версію)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Щоб дізнатися, як настроїти необов'язкові твердження, Дізнайтеся, [як надати до програми додаткові вимоги](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Щоб дізнатися, як використовувати атрибути розширення схем каталогів для надсилання даних користувача до програм у відповідних позовах, ознайомтеся [з атрибутами розширення схеми каталогів у позовах](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Щоб дізнатися, як настроїти тривалість маркера життя, ознайомтеся з [настроюванням маркера життя в платформі ідентифікації Microsoft (ознайомлювальну версію)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Настроювання політик тривалості життя маркера (ознайомлювальну версію)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – у цій статті ми пройтимемо за загальним сценарієм політики, за допомогою якого можна накладати нові правила для життя маркера. У цьому прикладі ви дізнаєтеся, як створити політику, яка вимагає, щоб користувачі могли перевіряти автентифікацію частіше в веб-програмі.

**Виправлення неполадок із конфігурацією єдиного входу**

- На запитання й відповіді про нетипові Sign-On (безшовні SSO) в [надбудові "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)для безшовних": запитання й відповіді.
- Щоб отримати відомості про поширені проблеми, пов'язані з нестандартними відомостями про "Лазурне" ("Лазурний") безшовні Sign-On (безшовне єдиного входу), перегляньте статтю [Виправлення неполадок із єдиним входом в Azure для Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
