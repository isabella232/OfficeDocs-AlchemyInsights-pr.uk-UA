---
title: Усунення проблем із єдиним входом в OIDC
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105805"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Усунення проблем із єдиним входом в OIDC

- Відомості про те, як додати програму на основі OIDC до клієнта Azure, див. в статті Короткий посібник. Настроювання єдиного входу на основі OIDC для програми в [клієнтах Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Докладні відомості про програми, які використовують стандарт OpenID Підключення для впровадження єдиного входу, див. в статтях Загальні відомості про єдиний вхід на основі [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Щоб отримати відомості про те, як написати код безпосередньо, надсилайте й обробляйте запити HTTP або використовуйте стороною бібліотеку з відкритим кодом, а не одну з наших бібліотек із відкритим кодом, див. в статтях [Протоколи OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)і OpenID Підключення на платформа ідентичностей Microsoft.

**Протоколи**

1. [платформа ідентичностей Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) і неявний потік надання – визначення характеристики неявного надання полягає в тому, що маркери (маркери ідентифікаторів або маркери доступу) повертаються безпосередньо з кінцевої точки /authorize замість кінцевої точки /token. Це часто використовується як частина потоку коду авторизації, що називається "гібридним потоком", щоб отримати маркер ідентифікатора в запиті **на /authorize** разом із кодом авторизації. У цій статті описано, як програма безпосередньо на основі протоколу у вашій програмі просити маркери з Azure AD.
2. платформа ідентичностей Microsoft і потік коду авторизації [OAuth 2.0.](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) Надати код авторизації OAuth 2.0 можна використовувати в програмах, інстальованих на пристрої, щоб отримати доступ до захищених ресурсів, наприклад веб-API. Використовуючи платформа ідентичностей Microsoft OAuth 2.0, можна додати вхід і доступ до API-інтерфейсу до мобільних і **класичних програм.** У цій статті описано, як запрошувати програму безпосередньо на протокол програми будь-якою мовою.
3. платформа ідентичностей Microsoft протоколи [та OpenID Підключення.](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) Якщо використовується платформа ідентичностей Microsoft впровадження OpenID Підключення, можна додати до програм доступ до входу та API. У цій статті описано, як це зробити незалежно від мови, а також описано, як надсилати й отримувати повідомлення HTTP без використання бібліотек із відкритим **кодом Microsoft.**
4. платформа ідентичностей Microsoft і потік облікових даних клієнта [OAuth 2.0.](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) Щоб отримати доступ до ресурсів, розміщених у веб-браузері, можна використовувати облікові дані клієнта OAuth 2.0, указані в RFC 6749 (інколи вони називають двома легендами **OAuth),** щоб отримати доступ до ресурсів, розміщених у веб-браузері, за допомогою ідентичності програми. Цей тип гранту зазвичай використовується для взаємодій між серверами, які мають виконуватися у фоновому режимі без негайної взаємодії з користувачем. Такі програми часто називають демонами або обліковими записами **служб.**  У цій статті описано, як програма безпосередньо проти протоколу у вашій програмі.
