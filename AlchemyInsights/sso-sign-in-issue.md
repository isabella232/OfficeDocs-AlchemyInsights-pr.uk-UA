---
title: Проблеми з входом користувача ЄДИНОГО входу
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935217"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Проблеми з входом користувача ЄДИНОГО входу

Після перевірки автентичності користувача браузер кешуватиме облікові дані користувача, щоб у той самий браузер програма автоматично ввійде в той самий обліковий запис. Це може ускладнити для іншого користувача або одного користувача для входу в кілька облікових записів на одному пристрої. Щоб вирішити цю проблему, зробіть ось що: 1. Виконайте вхід в інший браузер. 2. Очистьте кеш-пам'ять і/або файли cookie-браузера та повторіть спробу входу.

Якщо ви все ще відчуваєте проблеми з входом, радимо виконати діагностику та автоматизувати кроки роздільної здатності.

1. Інсталюйте [розширення браузера "мої програми](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) ", щоб отримати кращу діагностику та резолюції під час використання тестування на порталі "Лазурний".
2. Відтворіть помилку, використовуючи досвід тестування на сторінці конфігурації програми на порталі Azure. Докладні відомості наведено в статті [налагодження програм для входу в "САМЛ" на основі єдиної програми](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Якщо ви використовуєте досвід тестування на Лазуропорталі з розширенням захищеного браузера "мої програми", можна **пропустити крок 4**.
4. Щоб відкрити сторінку конфігурації єдиної входу на основі SAML, виконайте наведені нижче дії.
    - Відкрийте [портал "Лазурний](https://portal.azure.com/) " та увійдіть як **Глобальний адміністратор** або **coadmin**.
    - Відкрийте **розширення Azure Active Directory** , вибравши **всі служби** у верхній частині головного меню "перехід ліворуч".
    - У полі Пошук фільтра введіть "Блакитний Active Directory", а потім виберіть елемент " **Лазурне Active Directory** ".
    - Виберіть елемент **корпоративні програми** з меню "зліва" в області "розкривний каталог" з лівого боку.
    - Виберіть **Усі програми** , щоб переглянути список усіх програм. Якщо ви не бачите програму, яку потрібно відобразити тут, скористайтеся елементом керування **фільтром** у верхній частині **списку Усі програми** , а потім установіть прапорець **Показати** **всім застосункам**.
    - Виберіть програму, яку потрібно настроїти для одного входу.
    - Після завантаження програми виберіть елемент " **єдиний вхід** " з меню "у лівій частині програми".
    - Установіть прапорець **SSO для входу на основі SAML**.
5. На основі помилки, щоб дізнатися більше про Рекомендовані кроки, які слід стежити, перегляньте [проблеми з входом в настроєні програми для входу в "SAML" на основі єдиної реєстрації](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Щоб виправити неполадки інших проблем із входом користувача, ознайомтеся з такими вказівками:
    - [Єдина Sign-On-протокол SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Усунення помилок входу за допомогою звітів у службі Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Рядок несподіваної згоди](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Помилка згоди користувача](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Проблеми з входом з моїх програм](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Помилка на сторінці входу в програму](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Помилка під час входу в програму Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
