---
title: Віддалене вирішення проблем із підключенням до Windows 10 до Розширеного захисту від загроз для Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034055"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Віддалене вирішення проблем із підключенням до Windows 10 до Розширеного захисту від загроз для Microsoft Defender

Якщо ви можете отримати доступ до віддаленого комп'ютера, виконайте такі дії:

1. Завантажте [засіб діагностики підключення](https://go.microsoft.com/fwlink/?linkid=2143466) клієнта.
2. Видобути й запустити MDATPAnalyzer.cmd.
3. Знайдіть журнал діагностики в папці MDATPClientAnalyzerResult, яка є тією самою папку, у яку завантажено засіб аналізу.
4. Щоб знайти проблеми з підключенням або параметрами проксі-сервера в Інтернеті, перегляньте відомості про MDATPClientAnalyzer.txt.

Докладні відомості див. в [статтях Проблеми з прив'язаними машинами.](https://go.microsoft.com/fwlink/?linkid=2143634)
