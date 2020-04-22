---
title: Робота з iOS VPP додатків код правила 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719978"
---
# <a name="working-with-ios-vpp-applications"></a>Робота з додатками iOS VPP

Прочитайте, [як керувати додатками iOS, придбаними через програму купівлі-продажу з Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) , щоб дізнатися про функції, обмеження та кроки, щоб використовувати програму купівлі-продажу Apple і підтримку його в Microsoft InTune.
  
 **Поширені проблеми:** "Я призначив додаток iOS VPP для моїх користувачів, але установка не вдалося."
  
- Це може статися, якщо один маркер VPP використовується в кількох мобільних постачальників пристроїв керування. Маркери VPP від Apple можуть використовуватися лише з одним постачальником. Якщо ви використовували маркер VPP з кількома постачальниками, потрібно повторно завантажити маркер у InTune.

- Інсталяція також може не вдатися, якщо загальна кількість встановлень перевищує кількість ліцензій. Щоб переглянути звіт про використання для ліцензій, перейдіть на сторінку \> **ліцензії застосунку** для **мобільних додатків InTune** . Щоб дізнатися, як відновити використання ліцензій, див [у цій статті.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
