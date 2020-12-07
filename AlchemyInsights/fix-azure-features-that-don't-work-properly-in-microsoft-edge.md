---
title: Що робити, якщо функції Azure не працюють належним чином у Microsoft EDGE
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583778"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Що робити, якщо функції Azure не працюють належним чином у Microsoft EDGE

Microsoft EDGE має [відомі проблеми](https://go.microsoft.com/fwlink/?linkid=2140608) , пов'язані з зонами безпеки, і можуть вплинути на те, як у центрі адміністрування Windows є користувачі Azure. Якщо у вас виникли проблеми з використанням функцій Azure в Microsoft EDGE, виконайте наведені нижче дії.

1. У меню " **Пуск** " знайдіть пункт властивості **браузера** та виберіть його.
2. У діалоговому вікні **Властивості браузера** перейдіть на вкладку **Безпека** .
3. Виберіть зону **надійних сайтів** , а потім натисніть кнопку **сайти** .
4. У діалоговому вікні **Надійні веб-сайти** додайте URL-адресу шлюзу, а також [https://login.microsoftonline.com](https://login.microsoftonline.com) , а [https://login.live.com](https://login.live.com) потім натисніть кнопку **закрити**.
5. У діалоговому вікні **Властивості браузера** перейдіть на вкладку **конфіденційність** .
6. У розділі **блокування спливаючих вікон** натисніть кнопку **настройки**. У діалоговому вікні, що Відкриється, додайте URL-адресу шлюзу, а [https://login.microsoftonline.com](https://login.microsoftonline.com) також [https://login.live.com](https://login.live.com) , а потім натисніть кнопку **закрити**.
