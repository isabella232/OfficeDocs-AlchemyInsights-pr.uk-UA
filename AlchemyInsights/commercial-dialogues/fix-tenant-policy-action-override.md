---
title: Виправлення політики клієнта (перевизначення дії)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748984"
---
# <a name="fix-tenant-policy-action-override"></a>Виправлення політики клієнта (перевизначення дії)

Це повідомлення вплине на політику захисту від спаму в клієнті. Щоб переглянути політику, виконайте наведені нижче дії.

1. Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), а потім перейдіть до політики **керування загрозою**"  >    >  [Anti-спаму](https://go.microsoft.com/fwlink/?linkid=2101518)".
2. Перевірте, чи є **джерело політики** , що вказує на таке:  **Add-XHeader/Momesfyтема/переспрямування та видалення/без дій і прихованої копії повідомлення**

    Якщо так, на вкладці **Додатково** установіть прапорець настройки політики, які вплинули на повідомлення. Можливо, **стандартні параметри** , застосовані до всіх клієнтів Exchange Online Protection, вплинули на повідомлення.

Докладні відомості про настроювання політик фільтрування спаму наведено в статті [Настроювання політик фільтра спаму](https://go.microsoft.com/fwlink/?linkid=2101431).
