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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084367"
---
# <a name="sso-connection-issues"></a>Проблеми з підключенням до єдиного входу

1. Щоб налаштувати [програму, виконайте](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) вказівки з панелі швидкого запуску: настроювання властивостей посібника з програми.
2. Залежно від вибраної [програми](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) та параметра єдиного входу дотримуйтеся наведених нижче вказівок.
    - Відомості про  налаштування локальної програми для єдиного входу на основі SAML див. в розділі Єдиний вхід [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)для локальних програм за допомогою **проксі-сервера** програм .
    - Щоб дізнатися, як **настроїти хмарну** програму для єдиного входу на основі **пароля,** див. номери [Настроювання єдиного входу паролем.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Відомості про налаштування локальної програми для єдиного входу через **проксі-сервер** програм див. в розділі Зберігання паролів для єдиного входу за допомогою **проксі-сервера** [програм](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. Виправлення неполадок із **проксі-сервером** програми. Радимо почати з перевірки потоку виправлення [неполадок,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)які виникають у з'єднаторі проксі-сервера застосунку , щоб визначити, чи правильно настроєно з'єднатори проксі-сервера програм. Якщо проблеми з підключенням до програми не зникли, дотримуйтеся потоку виправлення неполадок у проблемах із проксі-сервером програми [налагодження.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Проблеми з [CORS можна виявити за](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) допомогою засобів налагодження браузера:
    - Запустіть браузер і перейдіть до веб-програми.
    - Натисніть **клавішу F12,** щоб відкрити консоль налагодження.
    - Спробуйте відтворити транзакцію та перегляньте повідомлення консолі. Порушення CORS призводить до помилки консолі про джерело.
    - Деякі проблеми з CORS не можна вирішити, наприклад коли програма переспрямує програму на login.microsoft.com для автентифікації, і термін дії маркера доступу завершиться. Після цього не вдасться виконати виклик CORS. Спосіб вирішення цієї ситуації – подовжити термін дії маркера доступу, щоб він не завершався під час сеансу користувача. Докладні відомості про те, як це зробити, див. в статті Час життя маркерів із настроюваним [платформа ідентичностей Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. Виправлення неполадок з єдиним входом на основі **SAML:** радимо перевірити проблеми із входом у настроєні програми на основі [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)щоб знайти вирішення проблем, які можуть виникнути.
5. **Виправлення неполадок, пов'язаних** із єдиним входом на основі пароля. Щоб знайти вирішення проблем, які можуть виникати, радимо перевірити, чи це єдиний вхід на основі пароля в [Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
6. Відомості про проблеми з підключенням під час використання мережі VPN див. в статті Використання єдиного входу [через мережу VPN і Wi-Fi з'єднаннями.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
