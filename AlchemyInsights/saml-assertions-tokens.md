---
title: Твердження SAML (маркери)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109261"
---
# <a name="saml-assertions-tokens"></a>Твердження SAML (маркери)

1. Маркери мови розмітки системи безпеки (SAML) – це представлення тверджень XML. За замовчуванням маркери SAML Windows communication Foundation (WCF) використовуються в федеративних сценаріях безпеки. Докладні відомості див. в [статтях Маркери SAML і Твердження.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. У платформа ідентичностей Microsoft виділяться кілька типів маркерів безпеки під час обробки кожного потоку автентифікації. [Посилання на твердження](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) маркерів SAML описує формат, характеристики безпеки та вміст маркерів SAML 2.0.
3. Дотримуйтеся вказівок у статті Настроюваний час життя маркерів у [платформа ідентичностей Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) щоб дізнатися, як настроїти час життя маркерів.
4. Виконайте вказівки з цієї [статті,](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) щоб дізнатися, як настроїти шифрування маркерів Azure AD SAML.
5. В Azure AD можна налаштувати параметри підписування сертифіката та алгоритм підписування сертифіката. Докладні відомості див. в розділі Додаткові параметри підписування сертифіката на [маркері SAML для програм колекції Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
