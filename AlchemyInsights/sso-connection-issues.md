---
title: Проблеми з підключенням до єдиного входу
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
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935207"
---
# <a name="sso-connection-issues"></a>Проблеми з підключенням до єдиного входу

1. Виконайте [QuickStart: Настройте властивості для посібника із програми,](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) щоб настроїти програму.
2. Залежно від вибраного [параметра "єдиний вхід](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ", виконайте відповідні вказівки нижче.
    - Щоб настроїти **локальну програму** для служби " **єдиний вхід на основі SAML**", перегляньте розділ " [єдиний вхід для локальних програм" за допомогою проксі-сервера програми](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Щоб настроїти **хмарну програму** для **входу на основі пароля**, перегляньте статтю  [настроїти єдиний вхід у пароль](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Щоб настроїти **локальну програму** для **окремого входу за допомогою проксі-сервера програми**, перегляньте статтю " [для входу паролем" за допомогою проксі-сервера програми "єдиний вхід](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)".
3. **Виправлення неполадок із проксі-сервером програми**: радимо розпочати перегляд потоку виправлення неполадок, [проблем із коннектором програми налагодження](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), щоб визначити, чи правильно настроєно сполучні лінії проксі-сервера програми. Якщо у вас все ще виникають проблеми з підключенням до програми, дотримуйтесь проблем із усууванням несправностей у розділі [проксі-застосунку програми налагодження](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Ви можете [визначити проблеми з CORORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) за допомогою інструментів налагодження браузера:
    - Запустіть браузер і перейдіть до веб-програми.
    - Натисніть клавішу **F12** , щоб відкрити консоль налагодження.
    - Виконайте спроби відтворити транзакцію та переглянути Консольне повідомлення. Під час порушення функції "Джерело" створюється помилка в консолі.
    - Деякі проблеми із входом не можна усунути, наприклад, коли програма переспрямовує на login.microsoft.com для автентифікації, а маркер доступу завершується. Під час виклику "виклики" не вдасться виконати виклик. Спосіб вирішення цього сценарію – подовжити термін дії маркера доступу, щоб запобігти його появі під час сеансу користувача. Щоб отримати докладні відомості про те, як це зробити, ознайомтеся [з Настроювана маркером користувача в платформі Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Виправлення неполадок на основі одного входу**: ми рекомендуємо перевіряти проблеми, які потрібно виконати, щоб знайти вирішення проблем, на [основі яких настроєно єдиний вхід для входу](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery).
5. **Виправлення неполадок під час входу на основі пароля**: ми радимо перевіряти [Виправлення неполадок під час входу на основі пароля в Лазурне AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), щоб знайти вирішення проблем, з якими ви, швидше за все, зіткнутися.
6. Щоб отримати проблеми з підключенням під час використання мережі VPN, Дізнайтеся, [як використовувати єдиний вхід (SSO) через VPN і Wi-Fi підключення](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
