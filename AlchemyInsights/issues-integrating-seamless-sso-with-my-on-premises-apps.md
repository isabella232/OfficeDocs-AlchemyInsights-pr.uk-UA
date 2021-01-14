---
title: Проблеми з інтеграцією безшовного входу в Локальні програми
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868771"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Проблеми з інтеграцією безшовного входу в Локальні програми

Щоб вирішити проблеми з інтеграцією безшовного входу в Локальні програми, виконайте наведені нижче дії.

**Рекомендовані дії**

1. Щоб настроїти **локальну програму** для **окремого входу за допомогою проксі-сервера програми**, перегляньте статтю " [для входу паролем" за допомогою проксі-сервера програми "єдиний вхід](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)".
1. **Виправлення неполадок із проксі-сервером програми**: радимо розпочати перегляд потоку виправлення неполадок, [проблем із коннектором програми налагодження](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), щоб визначити, чи правильно настроєно сполучні лінії проксі-сервера програми. Якщо ви все ще не змогли підключитися до програми, виконайте вказівки з виправлення неполадок у [вирішенні проблем програми налагодження проксі-](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)застосунку. За допомогою наведених нижче засобів відладки в браузері можна [визначити проблеми з CNAME](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) :
    1. Запустіть браузер і перейдіть до веб-програми.
    1. Натисніть клавішу **F12** , щоб відкрити консоль налагодження.
    1. Виконайте спроби відтворити транзакцію та переглянути Консольне повідомлення. Під час порушення функції "Джерело" створюється помилка в консолі.
    1. Деякі проблеми із входом не можна усунути, наприклад, коли програма переспрямовує на login.microsoftonline.com для автентифікації, а маркер доступу завершується. Під час виклику "виклики" не вдасться виконати виклик. Спосіб вирішення цього сценарію – подовжити термін дії маркера доступу, щоб запобігти його появі під час сеансу користувача. Щоб отримати докладні відомості про те, як це зробити, ознайомтеся [з Настроювана маркером користувача в платформі Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Рекомендовані документи**

- [Настроювання компонента "єдиний вхід у програму" для проксі-сервера програми](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Єдиний вхід для локальних програм із проксі-сервером програми](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Розуміння та вирішення проблем із проксі-сервером у службі "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Усунення несправностей у конфігурації делегування для протоколу Kerberos для проксі-сервера програми](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)