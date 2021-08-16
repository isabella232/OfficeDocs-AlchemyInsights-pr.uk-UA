---
title: Проблеми з інтегруванням щільного єдиного входу з локальними програмами
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028313"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Проблеми з інтегруванням щільного єдиного входу з локальними програмами

Щоб усунути проблеми з інтеграцюючого єдиного входу з локальними програмами, виконайте такі дії:

**Рекомендовані дії**

1. Відомості про налаштування локальної програми для єдиного входу через **проксі-сервер** програм див. в розділі Зберігання паролів для єдиного входу за допомогою **проксі-сервера** [програм](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Виправлення** неполадок із проксі-сервером програми. Ми радимо почати з перевірки потоку виправлення [неполадок,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)які виникають у з'єднаторі проксі-сервера застосунку , щоб визначити, чи правильно настроєно з'єднатори проксі-сервера програми. Якщо проблеми з підключенням до програми не зникли, виконайте дії з виправлення неполадок, описаних у статті Проблеми з проксі-сервером [програми налагодження.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Проблеми з [CORS можна виявити за](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) допомогою таких інструментів налагодження браузера:
    1. Запустіть браузер і перейдіть до веб-програми.
    1. Натисніть **клавішу F12,** щоб відкрити консоль налагодження.
    1. Спробуйте відтворити транзакцію та перегляньте повідомлення консолі. Порушення CORS призводить до помилки консолі про джерело.
    1. Деякі проблеми з CORS не можна вирішити, наприклад коли програма переспрямує програму на login.microsoftonline.com для автентифікації, і термін дії маркера доступу завершиться. Після цього не вдасться виконати виклик CORS. Спосіб вирішення цієї ситуації – подовжити термін дії маркера доступу, щоб він не завершався під час сеансу користувача. Докладні відомості про те, як це зробити, див. в статті Час життя маркерів із настроюваним [платформа ідентичностей Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Рекомендовані документи**

- [Настроювання єдиного входу в програму проксі-сервера програми](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Єдиний вхід SAML для локальних програм із проксі-сервером програми](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Вирішення проблем із Azure Active Directory проксі-серверів програм](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Усунення несправностей із конфігураціями обмеженого делегування Kerberos для проксі-сервера програм](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)