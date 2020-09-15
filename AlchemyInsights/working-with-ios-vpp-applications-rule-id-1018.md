---
title: Робота з програмами з iOS VPP для правил 1018
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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688967"
---
# <a name="working-with-ios-vpp-applications"></a>Робота з застосунками iOS VPP

Дізнайтеся, [як керувати програмами з iOS, придбаними за допомогою програми для придбання, за допомогою Microsoft Inteune](https://docs.microsoft.com/intune/vpp-apps-ios) , щоб дізнатися про функції, обмеження та кроки, щоб використовувати програму придбання Apple, а також підтримку для неї в Microsoft InTune.
  
 **Поширені проблеми:** "Я призначив програму iOS VPP для моїх користувачів, але Помилка інсталяції".
  
- Це може статися, якщо один маркер VPP використовується в різних провайдерів керування мобільними пристроями. Маркери VPP від Apple можна використовувати лише з одним постачальником. Якщо ви використовували маркер VPP із кількома постачальниками, потрібно повторно передати маркер на веб-програму Inune.

- Процес інсталяції також може не відповідувати, якщо загальна кількість інсталяцій перевищує кількість ліцензій. Щоб переглянути звіт про використання ліцензій, перейдіть на сторінку ліцензії програми для **мобільних пристроїв програми inune** \> **App licenses** . Щоб дізнатися, як відновити ліцензії у використанні, ознайомтеся з [цією статтею.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
