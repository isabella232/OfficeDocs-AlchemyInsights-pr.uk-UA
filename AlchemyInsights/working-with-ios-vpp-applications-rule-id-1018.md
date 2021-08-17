---
title: Робота з кодом правила VPP для iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083035"
---
# <a name="working-with-ios-vpp-applications"></a>Робота з програмами VPP для iOS

У статті Керування програмами [для iOS,](https://docs.microsoft.com/intune/vpp-apps-ios) придбаними за програмою корпоративного придбання в Microsoft Intune, щоб дізнатися про функції, обмеження та кроки, які потрібно виконати в програмі Apple Volume Purchase Program, і підтримку для цієї програми Microsoft Intune.
  
 **Поширені проблеми:** "Користувачам призначено програму VPP для iOS, але не вдалося виконати інсталяцію".
  
- Це може статися, якщо один маркер VPP використовується в кількох постачальників послуг керування мобільними пристроями. Маркери VPP від Apple можна використовувати лише в одного постачальника. Якщо ви використовували маркер VPP із кількома постачальниками, потрібно повторно передати маркер в Intune.

- Інсталяція також може не вдатися, якщо загальна кількість інсталяцій перевищує кількість ліцензій. Щоб переглянути звіт про використання ліцензій, перейдіть на сторінку Ліцензії на програми **Intune** \>  Mobile. Щоб дізнатися, як відклскати ліцензії, які використовуються, [див. цю статтю.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
