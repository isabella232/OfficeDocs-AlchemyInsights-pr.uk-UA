---
title: Single-Sign для пристроїв, підключених до Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405665"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Єдиний вхід для пристроїв, підключених до Azure Active Directory

Якщо у вас є локальне середовище Active Directory (AD) і ви хочете приєднатися до комп'ютерів, приєднаних до домену, до Azure AD, це можна зробити, виконавши гібридне приєднання Azure AD. [Інструкції.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Сплануйте гібридне впровадження Azure Active Directory, виконавши відповідні кроки, щоб реалізувати гібридне об'єднання Azure AD у вашому середовищі.

[Налаштування приєднаних пристроїв до Azure AD для локальних Single-Sign за допомогою Windows Hello для бізнесу](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Проблеми з основним маркером оновлення (PRT)** Основний маркер оновлення (PRT) – це основний артефакт автентифікації Azure AD у Windows 10, Windows Server 2016 і пізніших версій, iOS і Android. Це маркер JSON Web Token (JWT), який спеціально видано брошурам корпорації Майкрософт із маркерами першої сторони, щоб активувати єдиний вхід (SSO) для всіх програм, які використовуються на цих пристроях. [У статті Що таке](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)основний маркер оновлення? ми надамо докладні відомості про те, як видано, використовується та захищається PRT на пристроях із Windows 10.

**WamDefaultSet: YES і AzureADPrt: YES** Ці поля вказують, чи користувач успішно автентифікувався в Azure AD під час входу на пристрій. Якщо значення мають значення **NO (НІ),** це може бути пов'язано з терміном виконання:

- Хибний ключ сховища в TPM, пов'язаному з пристроєм під час реєстрації (перевірте KeySignTest під час запуску влітку).
- Додатковий ідентифікатор входу
- Проксі-сервер HTTP не знайдено

Усунення несправностей пристроїв за допомогою команди dsregcmd – [стан єдиного входу](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
