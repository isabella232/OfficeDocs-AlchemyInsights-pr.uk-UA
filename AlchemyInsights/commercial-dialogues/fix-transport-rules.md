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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750570"
---
# <a name="fix-transport-rules"></a>Виправлення правил транспортування

Це повідомлення вплинуло на настроюване правило потоку пошти. Щоб переглянути точне правило, виконайте наведені нижче дії.

1. У результатах надсилання в розділі **додаткові відомості** зверніть увагу на **ідентифікатор GUID** або **ім'я політики**.
2. Запуск оболонки керування Exchange. Докладні відомості наведено в статті [відкриття оболонки керування Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Виконати цю команду (за допомогою ідентифікатора GUID у поданні):  **Get-Transportule-ідентичність "GUID" | FL * Опис***
4. Перегляньте опис, щоб переглянути настроєні умови, які вплинули на повідомлення.

Щоб дізнатися більше, перегляньте статтю [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
