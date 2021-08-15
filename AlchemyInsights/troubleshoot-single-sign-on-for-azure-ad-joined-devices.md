---
title: Усунення несправностей із єдиним входом для приєднаних пристроїв Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039267"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Усунення несправностей із єдиним входом для приєднаних пристроїв Azure AD

Якщо у вас є локальне середовище Active Directory (AD) і ви хочете приєднатися до комп'ютерів, приєднаних до домену, до Azure AD, це можна зробити, виконавши гібридне приєднання Azure AD. [Інструкції.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Планування гібридного середовища Azure Active Directory приєднання надає відповідні кроки з упровадження гібридного об'єднання Azure AD в середовищі.

Докладні відомості див. в Single-Sign Налаштування приєднаних до служби Azure AD пристроїв Single-Sign [у Windows Hello для бізнесу.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Проблеми з основним маркером оновлення (PRT)**

Основний маркер оновлення (PRT) – це основний артефакт автентифікації Azure AD на пристроях Windows 10, Windows Server 2016 і пізніших версій, iOS і Android. Це маркер JSON Web Token (JWT), який спеціально видано брошурам корпорації Майкрософт із маркерами першої сторони, щоб активувати єдиний вхід (SSO) для всіх програм, які використовуються на цих пристроях. Докладні відомості про те, як видано, використовується та захищено PRT на пристроях із Windows 10, див. в статті Що таке основний маркер [оновлення?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES і AzureADPrt: YES**

Ці поля вказують, чи користувач успішно автентифікувався в Azure AD під час входу на пристрій. Якщо значення мають значення **NO**, можливо, це пов'язано з такою причиною:

- Хибний ключ сховища в TPM, пов'язаному з пристроєм під час реєстрації (перевірте KeySignTest під час запуску влітку)
- Додатковий ідентифікатор входу
- Проксі-сервер HTTP не знайдено

Відомості про виправлення неполадок пристроїв за допомогою команди dsregcmd див. в цьому [стані.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
