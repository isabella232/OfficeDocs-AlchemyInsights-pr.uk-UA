---
title: Усунення несправностей, пов'язаних із паролем під час єдиного входу
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972845"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Усунення несправностей, пов'язаних із паролем під час єдиного входу

Щоб дізнатися про ґрунтові принципи використання єдиного входу на основі пароля, див. номери автентифікації за [допомогою Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Настроювання єдиного входу на основі пароля**

1. [Настроювання єдиного входу](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) на основі пароля. У цій статті докладно описано параметри єдиного входу на основі пароля. Якщо для програми, яку ви додаєте, потрібна спеціальна конфігурація та потрібно використовувати єдиний доступ на основі пароля, ця стаття саме для вас.
2. [Налаштування єдиного входу на основі пароля для програм,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) що підтримуються в онлайновому розгорнутому вікні. Проксі-сервер програми підтримує кілька режимів єдиного входу. Вхід за допомогою пароля призначено для програм, які використовують комбінацію з іменем користувача та паролем для автентифікації. Під час налаштування входу в програму на основі пароля користувачі мають один раз увійти в локальну програму. Після цього Azure Active Directory відомості для входу зберігаються та автоматично надається програмі, коли користувачі отримувати доступ до неї віддалено.
    - Ви вже опублікували й протестували програму з проксі-сервером програми. Якщо ні, виконайте кроки, описані в статті Публікування програм за допомогою проксі-сервера програм [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) а потім продовжте настроювання єдиного входу на основі пароля для доступних програм.

Щоб дізнатися, як виправити неполадки єдиного входу на основі пароля, див. номери виправлення неполадок єдиного входу на основі [пароля в Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
