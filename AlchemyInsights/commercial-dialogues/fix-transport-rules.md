---
title: Виправлення правил транспортування
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034775"
---
# <a name="fix-transport-rules"></a>Виправлення правил транспортування

Настроюване правило пересилання пошти, на яке впливає це повідомлення. Щоб перевірити точне правило, виконайте такі дії:

1. У результатах надсилання в розділі **Додаткові** відомості зверніть увагу на **GUID** або **ім'я політики.**
2. Запустіть Exchange Керування. Докладні відомості [див. в сторінці Відкриття оболонки Exchange керування.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Виконайте цю команду (за допомогою GUID із надсилання):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Перегляньте опис, щоб переглянути настроєні умови, які впливають на повідомлення.

Докладні відомості див. в [статтях Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
