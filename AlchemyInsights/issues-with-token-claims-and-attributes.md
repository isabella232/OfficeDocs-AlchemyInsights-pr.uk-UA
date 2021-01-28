---
title: Проблеми з відповідними вимогами і атрибутами маркерів
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036081"
---
# <a name="issues-with-token-claims-and-attributes"></a>Проблеми з відповідними вимогами і атрибутами маркерів

**Оновлення, настроювання та видалення тверджень про маркер**

1. Використовуючи Azure Active Directory (Azure AD), можна [Настроїти тип твердження для твердження про роль](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) у відповіді, який ви отримали після авторизації програми.
2. Розробники програм можуть використовувати необов'язкові претензії в своїх програмах Azure AD, щоб указати, які претензії вони хочуть в маркери, які надходять до їх програми. Додаткові відомості наведено в статті [надання необов'язкових претензій до програми](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Настройте вимоги до груп для програм за допомогою служби Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Якщо у вашій програмі використовується небезшовний єдиний вхід, див. розділ ["настроїти претензії, видані в маркер SAML для корпоративних програм"](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Зіставлення атрибутів тверджень**

1. Щоб настроїти політику зіставлення тверджень за допомогою PowerShell, перегляньте статтю [настроїти претензії, що випускаються в маркерів для певної програми в клієнті (ознайомлювальну версію)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Атрибути розширення схеми каталогів дають змогу зберігати додаткові дані в Лазурому Active Directory на об'єктах користувача та інших об'єктах каталогу, як-от групи, відомості про клієнта, керівники служб. Для застосування позовів до програм можна використовувати лише атрибути розширення для об'єктів користувача. [За допомогою атрибутів розширення схем каталогів у позовах](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) розповідається про те, як використовувати атрибути розширення схем каталогів для надсилання даних користувача до програм у позовах маркерів.

Докладні відомості про твердження маркерів наведено в статті:

- [Скарги в маркери доступу](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Скарги в id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Твердження](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) про те, що ви можете розраховувати на маркери ідентифікаторів і маркери доступу, видані за допомогою AZURE AD B2C
- [Довідник із маркерів "САМЛ"](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
