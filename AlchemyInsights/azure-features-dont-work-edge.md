---
title: Що робити, якщо функції Azure працюють неправильно в Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812882"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Що робити, якщо функції Azure працюють неправильно в Microsoft Edge

Microsoft Edge має відомі проблеми, пов'язані зі зонами безпеки, які можуть вплинути на вхід у Windows адміністрування Azure. Докладні відомості див. в [довідці з відомих проблем у Edge.](https://go.microsoft.com/fwlink/?linkid=2140608) Якщо у вас виникають проблеми з використанням функцій Azure Microsoft Edge, спробуйте зробити ось що:

1. На меню в **рядку пошуку** введіть **Властивості браузера**, а потім виберіть його.
1. У **розділі Властивості браузера** виберіть **вкладку** Безпека.
1. Виберіть **надійні сайти**, а потім – **Сайти**.
1. Додайте URL-адресу шлюзу, а <https://login.microsoftonline.com> також і натисніть кнопку <https://login.live.com> **Закрити**.
1. У **розділі Властивості браузера** виберіть вкладку **Конфіденційність.**
1. У розділі Блокувальник спливаючих об'Настройки **.** Додайте URL-адресу шлюзу, а <https://login.microsoftonline.com> також і натисніть кнопку <https://login.live.com> **Закрити.**