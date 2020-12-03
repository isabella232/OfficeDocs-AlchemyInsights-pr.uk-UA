---
title: Помилка ліцензії на кінцеву точку DLP
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564873"
---
# <a name="endpoint-dlp-licensing-error"></a>Помилка ліцензії на кінцеву точку DLP

Під час спроби настроїти кінцеву точку DLP, якщо ви отримали таке повідомлення про помилку:

`Your organization is missing the licenses required to manage these devices`.

Переконайтеся, що ви маєте одну з таких передплат або додаткових компонентів:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Відповідність Microsoft 365 E5
- Відповідність вимогам служби Microsoft 365 a5
- Служба захисту та керування даними Microsoft 365 E5
- Захист і керування інформацією в Microsoft 365 a5

> [!NOTE]
> Це не спрацює для комбінацій ліцензій, наприклад: Win E5 + O365 E5 + EMS E5. Щоб налаштувати цю функцію, потрібно мати ліцензію чистої M365 E5.

Щоб отримати додаткові відомості про ліцензування DLP, перегляньте статтю [ЛІЦЕНЗУВАННЯ DLP для кінцевих точок.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
