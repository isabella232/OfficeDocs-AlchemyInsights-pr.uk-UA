---
title: Помилка ліцензування DLP кінцевої точки
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090181"
---
# <a name="endpoint-dlp-licensing-error"></a>Помилка ліцензування DLP кінцевої точки

Якщо під час спроби налаштувати DLP кінцевої точки з'являється таке повідомлення про помилку:

`Your organization is missing the licenses required to manage these devices`.

Переконайтеся, що у вас є одна з таких передплат або додаткові компоненти:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 відповідності вимогам
- Microsoft 365 A5 відповідності вимогам
- Microsoft 365 E5 захисту та керування інформацією
- Microsoft 365 A5 захисту та керування інформацією

> [!NOTE]
> Це не працює для комбінацій ліцензій, наприклад: Win E5 + O365 E5 + EMS E5. Щоб налаштувати цю функцію, потрібно мати чисту ліцензію M365 E5.

Докладні відомості про ліцензування DLP кінцевих точок див. в відомості про [ліцензування DLP кінцевої точки.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
