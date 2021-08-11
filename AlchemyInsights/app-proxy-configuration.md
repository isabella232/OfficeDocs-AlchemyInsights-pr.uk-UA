---
title: Конфігурація проксі-сервера програми
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951586"
---
# <a name="app-proxy-configuration"></a>Конфігурація проксі-сервера програми

1. Щоб дізнатися, як налаштувати проксі-сервер програм в Azure AD так, щоб локальні програми стояли в хмарі, див. номери настроювання проксі-сервера [програм](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Єдиний вхід (SSO) дає змогу користувачам отримувати доступ до програми, не проходячи автентифікацію кілька разів. Вона дає змогу здійснювати єдину автентифікацію в хмарі на Azure Active Directory і дає змогу службі або з'єднувачу узагальнити користувача, щоб виконати будь-які додаткові проблеми з автентифікацією в програмі. Докладні відомості див. в статті Настроювання єдиного входу в [програму проксі-сервера програми.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Скористайтеся [цією статтею,](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) щоб усунути поширені проблеми зі створенням проксі-сервера в програмі.
4. Якщо виникають проблеми під час налаштування серверної автентифікації в програмі, можливо, знадобиться виправити неполадки конфігурацій обмежених делегування [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) для проксі-сервера програм або дотримуйтеся вказівок із настроювання програми за допомогою [PingAccess,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) щоб вирішити проблему.
