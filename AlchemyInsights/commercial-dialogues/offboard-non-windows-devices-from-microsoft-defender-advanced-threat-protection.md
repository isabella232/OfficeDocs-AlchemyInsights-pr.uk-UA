---
title: Offboard непристроїв із Windows від засобу захисту від досвідчених загроз Microsoft Defender (АТФ)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748487"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard непристроїв із Windows від засобу захисту від досвідчених загроз Microsoft Defender (АТФ)

Ось як це зробити.

1. Виконайте документацію третьої сторони, щоб від'єднатися від стороннього рішення від компанії Microsoft Defender АТФ.
2. З клієнта Azure Active Directory, видаліть дозволи для рішення стороннього виробника.

    1. Увійдіть на [портал Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Виберіть **Усі служби**"  >  **блакитні активні каталоги**" для  >  **корпоративних програм**.
    1. Виберіть програму, яку потрібно додати до offboard.
    1. Натисніть кнопку **Видалити**.

Докладні відомості можна знайти в [надбудові offboard, що не є пристроями для Windows](https://go.microsoft.com/fwlink/?linkid=2143630).
