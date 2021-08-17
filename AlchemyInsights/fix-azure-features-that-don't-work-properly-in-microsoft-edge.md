---
title: Що робити, якщо функції Azure працюють неправильно в Microsoft Edge
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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117109"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Що робити, якщо функції Azure працюють неправильно в Microsoft Edge

Microsoft Edge має [відомі проблеми,](https://go.microsoft.com/fwlink/?linkid=2140608) пов'язані з зонами безпеки, і може вплинути на спосіб входу користувачів Azure Windows адміністрування. Якщо у вас виникають проблеми з використанням функцій Azure Microsoft Edge, спробуйте зробити ось що:

1. У меню **Пуск** знайдіть пункт **Властивості браузера** та виберіть його.
2. У **діалоговому вікні** Властивості браузера перейдіть на **вкладку Безпека.**
3. Виберіть **зону Надійні** веб-сайти, а потім натисніть **кнопку** Сайти.
4. У **діалоговому вікні Надійні** веб-сайти додайте URL-адресу шлюзу, а також [https://login.microsoftonline.com](https://login.microsoftonline.com) і натисніть кнопку [https://login.live.com](https://login.live.com) **Закрити.**
5. У **діалоговому вікні** Властивості браузера перейдіть на вкладку **Конфіденційність.**
6. У розділі **Блокувальник спливаючих об'Настройки** **.** У діалоговому вікні, що відкриється, додайте URL-адресу свого шлюзу, а також [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) і натисніть кнопку **Закрити.**
