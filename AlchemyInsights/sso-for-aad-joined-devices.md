---
title: Single-Sign ввімкнено для Azure Active Directory приєднаних пристроїв
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050031"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Єдиний вхід для Azure Active Directory приєднаних пристроїв

Якщо у вас є локальне середовище Active Directory (AD) і ви хочете приєднатися до комп'ютерів, приєднаних до домену, до Azure AD, це можна зробити, виконавши гібридне приєднання Azure AD. [Інструкції.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Планування гібридного середовища Azure Active Directory приєднання надає відповідні кроки з упровадження гібридного об'єднання Azure AD в середовищі.

[Налаштування приєднаних пристроїв до Azure AD для локальної служби Single-Sign Увімк. Windows Hello для бізнесу](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Проблеми з основним маркером оновлення (PRT)** Основний маркер оновлення (PRT) – це основний артефакт автентифікації Azure AD на пристроях Windows 10, Windows Server 2016 і пізніших версій, iOS і Android. Це маркер JSON Web Token (JWT), який спеціально видано брошурам корпорації Майкрософт із маркерами першої сторони, щоб активувати єдиний вхід (SSO) для всіх програм, які використовуються на цих пристроях. [У статті Що таке](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)основний маркер оновлення? ми надамо докладні відомості про те, як видано, використовується та захищається PRT на Windows 10 пристроях.

**WamDefaultSet: YES і AzureADPrt: YES** Ці поля вказують, чи користувач успішно автентифікувався в Azure AD під час входу на пристрій. Якщо значення мають значення **NO (НІ),** це може бути пов'язано з терміном виконання:

- Хибний ключ сховища в TPM, пов'язаному з пристроєм під час реєстрації (перевірте KeySignTest під час запуску влітку).
- Додатковий ідентифікатор входу
- Проксі-сервер HTTP не знайдено

Усунення несправностей пристроїв за допомогою команди dsregcmd – [стан єдиного входу](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
