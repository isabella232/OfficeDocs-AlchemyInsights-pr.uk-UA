---
title: Робота з iOS очок VPP додатків правило Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917517"
---
# <a name="working-with-ios-vpp-applications"></a>Робота з iOS очок VPP додатків

Читав, [як керувати iOS застосунки, придбані через обсяг купівлі програми з Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) щоб дізнатися про особливості, обмеження та кроки, щоб зробити використання Apple обсяг купівлі програми та підтримку для його в Microsoft Intune. 
  
 **Поширених проблем:** "Я призначено застосунок очок VPP iOS мої користувачі, але не установка". 
  
- Це може статися, якщо використання єдиного очок VPP маркера через декілька провайдерів мобільного пристрою управління. ВПП токени від Apple можна використовувати лише з одного постачальника. Якщо ви використовували очок VPP маркер з кількох джерел, потрібно повторно завантажувати токен до Intune.
    
- Установка може також виникає, якщо загальна кількість установок перевищує кількість ліцензій. Щоб переглянути використання звіт для вашої ліцензії, перейдіть на **Intune мобільних додатків** \> **ліцензії застосунку** сторінки. Щоб відновити ліцензій на використання, розділ [цю статтю.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

