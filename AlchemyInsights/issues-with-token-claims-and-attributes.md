---
title: Проблеми з твердженнями маркерів і атрибутами
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012905"
---
# <a name="issues-with-token-claims-and-attributes"></a>Проблеми з твердженнями маркерів і атрибутами

**Оновлення, настроювання та вилучення тверджень маркерів**

1. За допомогою Azure Active Directory (Azure AD) [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) можна настроїти тип претензій на роль у маркері відповіді, отриманому після авторизації програми.
2. Розробники програм можуть використовувати додаткові вимоги в програмах Azure AD, щоб указати, які вимоги мають бути в маркерах, надісланих у своїй програмі. Докладні відомості див. в [статтях Надання додаткових претензій для програми.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Настройте групові твердження для програм за допомогою Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Якщо у вашій програмі використовується без проблем під час єдиного входу, перегляньте настроювання вимог, виданих у маркері [SAML для корпоративних програм.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Зіставлення атрибутів тверджень**

1. Відомості про налаштування політики зіставлення тверджень за допомогою PowerShell див. в розділі Налаштування тверджень, які вимагаються в маркерах певної програми в попередньому [перегляді клієнта.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Атрибути розширення схеми каталогу дають користувачам Azure Active Directory дані в об'єктах користувача та інших об'єктах каталогу, як-от групах, відомості про клієнта, основних відомості про службу. Для випромінення претензій до програм можна використовувати лише атрибути розширення об'єктів користувачів. [Використання атрибутів](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) розширення схеми каталогів у твердженнях описує, як надсилати дані користувачів до програм у твердженнях маркерів за допомогою атрибутів розширення схеми каталогів.

Докладні відомості про вимоги маркерів див. в статтях:

- [Твердження в маркерах доступу](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Претензії на id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Твердження,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) які можна очікувати в маркерах ідентифікаторів і маркерах доступу, виданих Azure AD B2C
- [Довідник із тверджень про маркери SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
