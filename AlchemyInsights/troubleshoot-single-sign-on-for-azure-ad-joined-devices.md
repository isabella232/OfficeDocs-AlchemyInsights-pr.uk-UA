---
title: Виправлення неполадок із одинарним входом для пристроїв, підключених до мережі Azure
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037337"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Виправлення неполадок із одинарним входом для пристроїв, підключених до мережі Azure

Якщо у вас є локальна Служба Active Directory (AD), і ви хочете приєднатися до свого домену, до якого приєдналися комп'ютери з лазуровим ОГОЛОШЕННЯМ, можна виконати цю роботу, виконавши гібридне об'єднання Лазур. [Планування гібридного використання служби "Блакитний" для Active Directory –](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) надання вам відповідних заходів для реалізації гібридного об'єднання Azure в навколишньому середовищі.

Докладні відомості наведено в статті [Настроювання пристроїв AZURE AD для локального Single-Sign з використанням Windows Hello для бізнесу](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Проблеми з основним маркером оновлення (PRT)**

Основний маркер оновлення (PRT) – ключовий артефакт автентифікації в Azure AD в ОС Windows 10, Windows Server 2016 і новіших версіях, iOS і Android. Це веб-маркер JSON (JWT), спеціально виданий для брокерів від корпорації Майкрософт першого учасника, щоб активувати єдиний вхід (SSO) через програми, які використовуються на цих пристроях. Докладні відомості про те, як видається ГВП, використовується та захищена на пристроях з ОС Windows 10, Дізнайтеся, [що таке первинний маркер оновлення?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet набору: так і AzureADPrt: так**

Ці поля вказують, чи користувач успішно автентифіковано для Azure AD під час входу на пристрій. Якщо значення **немає**, це може бути пов'язано з такими значеннями:

- Хибний ключ сховища в модулі TPM, пов'язаний із пристроєм під час реєстрації (перевірка KeySignTest під час роботи з підвищеною)
- Альтернативний ІДЕНТИФІКАТОР входу
- Проксі-сервер HTTP не знайдено

Щоб виправити неполадки на пристроях за допомогою команди dsregcmd, ознайомтеся з пунктом " [стан єдиного входу](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)".
