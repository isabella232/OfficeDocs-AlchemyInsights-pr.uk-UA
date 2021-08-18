---
title: 2681 Атака Simulator Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325092"
---
# <a name="attack-simulator-in-microsoft-365"></a>Моделятор атаки в Microsoft 365

- Не бракує симулятора атаки? Для моделювання атаки потрібен **Захисник Microsoft Office 365 (план 2** **або Office 365 для підприємств E5).** Моделятор  атаки не входить до складу Захисника Microsoft Office 365 (план 1, Office 365 для підприємств E3 або будь-Програми Microsoft 365 для бізнесу передплати).

- Для запуску зімітованих атак облікового запису потрібні дозволи глобального адміністратора або адміністратора безпеки та багатофакторна автентифікація (MFA). Докладні відомості про вимоги до моделювання атаки див. [в цій статті.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Важливі відомості про **Brute Force Password attack** simulations:

  - Якщо для цільового облікового запису активовано багатофакторну автентифікацію, а пароль вдасться вгадати правильно, обліковий запис не відображатимуться як злам (другий фактор автентифікації буде неповний).

  - Розмір файлу пароля не має бути більше 10 МБ. У кожного рядка слід використовувати один пароль і включати пустий рядок (повернення карети) після останнього пароля в списку.

- Важливі відомості про **моделювання фішингів:**

  - За задумом не можна вказати настроюване значення для URL-адреси сервера **фішинг для входу.**

  - Якщо одержувач використовує [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) надбудову "Активувати звіт про повідомлення", щоб повідомити про фішинг, повідомлення може не надійти (оскільки це зімітована атака).

- Звіти. Після зімітованої атаки можна натиснути кнопку Відомості про **атаку,** щоб переглянути звіт.

- Докладні інструкції та нові функції в симуляторі атаки див. в статті [Моделятор атаки в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
