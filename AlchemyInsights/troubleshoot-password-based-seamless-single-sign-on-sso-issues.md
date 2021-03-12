---
title: Виправлення неполадок із надбудовами для єдиного входу на основі пароля (SSO)
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714891"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Виправлення неполадок із надбудовами для єдиного входу на основі пароля (SSO)

Щоб дізнатися основи єдиного входу на основі пароля, ознайомтеся [з автентифікацією на основі пароля за допомогою служби Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Настроювання єдиного входу на основі пароля**

1. [Настроювання єдиного входу на основі пароля](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – у цій статті описано докладні відомості про параметр SSO на основі пароля. Якщо програма, яку потрібно додати, потребує настроюваної конфігурації, і вам потрібно використовувати службу єдиного входу на основі пароля, щоб ця стаття була для вас.
2. [Настроїти єдиний вхід на основі пароля для програм для роботи з іншими програмами](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – проксі-застосунок підтримує кілька режимів входу. Вхід на основі пароля призначено для програм, які використовують комбінацію імені користувача та пароля для автентифікації. Під час настроювання входу на основі пароля для програми користувачі мають входити в локальну програму. Після цього Лазур Active Directory зберігає інформацію про вхід і автоматично надає його програмі, коли користувачі мають доступ до нього віддалено.
    - Ви вже маєте публікувати та перевіряти програму за допомогою проксі-сервера програми. Якщо ні, виконайте вказівки, описані в статті [публікування програм за допомогою проксі-сервера служби Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , а потім Продовжіть КОНФІГУРАЦІЮ єдиного входу на основі пароля для програм для роботи з надбудовами.

Щоб виправити виправлення ЄДИНОГО входу на основі пароля, перегляньте статтю [Виправлення неполадок із входом на основі пароля в Лазурне AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
