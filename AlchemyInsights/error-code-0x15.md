---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 на розгортання служб віддалених робочих столів (RDS), спробуйте увімкнути ADAL, редагуючи реєстр.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703159"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Помилка під час активації Office 2013 на службах віддалених робочих столів

Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 на розгортання служб віддалених робочих столів (RDS), спробуйте увімкнути ADAL, редагуючи реєстр.
  
|**Реєстру**|**Тип**|**Значення**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Щоб отримати додаткові відомості див. [Увімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL увімкнуто за промовчанням у програмах Microsoft 365 для підприємств і Office 2016. Служби віддалених робочих столів (RDS) раніше називали служби терміналів.
  