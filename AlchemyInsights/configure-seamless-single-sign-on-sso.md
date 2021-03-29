---
title: Настроювання нескладного єдиного входу (SSO)
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
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402288"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Настроювання нескладного єдиного входу (SSO)

**Настроювання програм**

1. Значення слід отримувати від постачальника програми. Ви можете вручну ввести значення або передати файл метаданих, щоб видобути значення полів.
2. Багато програм уже попередньо налаштовано для роботи з Azure AD. Ці програми наведено в колекції програм, які можна переглянути під час додавання програми до клієнта Azure AD. У [короткому посібнику](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) з'являться покроки, які потрібно пройти.
3. Щоб створити програму, яка не є колекцією, натисніть кнопку **+ Створити** власну кнопку програми та дайте ім'я своїй програмі.
    - За замовчуванням вона вибере **пункт** Інтегрувати будь-яку іншу програму, якої немає в колекції, яка є правильним варіантом для програм, які не надається в колекції.
    - Коли ви **натиснете** кнопку Створити, коли введете ім'я для програми, буде створено новий корпоративний застосунок, який не є колекцією.
    - Потім у розділі Керування  програмою можна  перейти до кнопки Єдиний вхід і переглянути різні методи її впровадження в середовищі.

**Налаштування несмісного єдиного входу для певної програми**

Для програм у колекції ви знайдете докладні покрокові вказівки. Щоб отримати доступ до кроків, ви можете переглянути список усіх посібників із конфігурації програм на сторінці Посібники з настроювання [програми SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Настроювання єдиного входу на основі SAML**

1. [Короткий посібник.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)Настроювання єдиного входу на основі SAML для програми в клієнта Azure Active Directory (Azure AD).
2. Докладні відомості про параметр на основі SAML для єдиного входу див. в статтях Загальні відомості про єдиний вхід на [основі SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Щоб дізнатися про запити на автентифікацію SAML 2.0 і відповіді, які підтримуються в службі Azure Active Directory (Azure AD) для єдиного входу Sign-On (SSO), див. Sign-On протокол [SAML.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Щоб дізнатися, як створити та настроїти єдиний вхід на основі SAML для програми в Azure Active Directory (Azure AD) за допомогою API Microsoft Graph, див. номери Настроювання єдиного входу на основі SAML для програми за допомогою [Microsoft Graph API.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Відомості про те, як Azure AD використовує протокол SAML, див. в статті Використання протоколу [SAML на платформі Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Настроювання маркерів і вимог**

1. [Інструкції: настроювання тверджень, виданих у маркері SAML для корпоративних програм.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Відомості про те, як налаштувати твердження за допомогою PowerShell, див. в статті Налаштування тверджень, що вимагаються маркерами для певної програми в ознайомлювальної [версії клієнта.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Щоб дізнатися, як додатково настроїти вимоги, див. діяти як: указати додаткові вимоги [для програми.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Щоб дізнатися, як за допомогою атрибутів розширення схеми каталогів надсилати дані користувачів застосункам у твердження щодо маркера, див. номери атрибутів розширення схеми каталогу в [твердженнях.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Відомості про те, як налаштувати час життя маркерів, див. в статті Час життя маркерів, що можна настроювати на платформі ідентичності [Microsoft (ознайомча версія).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Налаштуйте політики часу життя](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) маркерів (попередній перегляд). У цій статті описано типовий сценарій політики, який допоможе настроювати нові правила для терміну служби маркерів. У прикладі ви дізнаєтеся, як створити політику, яка вимагає, щоб користувачі автентифікуватимуться частіше у веб-програмі.

**Усунення несправностей із конфігурацією єдиного**

- Запитання й відповіді про Azure Active Directory про єдиний вхід Sign-On (без проблемний єдиний вхід) див. в запитаннях і відповідей про єдиний вхід в [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Відомості про виправлення неполадок, пов'язаних із Azure Active Directory (Azure AD), див. в Sign-On єдиного входу в [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
