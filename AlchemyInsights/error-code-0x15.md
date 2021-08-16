---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Якщо під час активації пакета Office 2013 у розгортань служб віддалених робочих столів (RDS) з'являється повідомлення про помилку, редагуючи реєстр, можна активувати ADAL.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100783"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Помилка під час активації Office 2013 у службах віддалених робочих столів

Якщо під час активації пакета Office 2013 у розгортань служб віддалених робочих столів (RDS) з'являється повідомлення про помилку, редагуючи реєстр, можна активувати ADAL.
  
|**Розділ реєстру**|**Тип**|**Значення**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Докладні відомості див. в сторінці [Активація сучасної автентифікації Office 2013 на Windows пристроях.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  AdAL активовано за замовчуванням у Програми Microsoft 365 для підприємств 2016 Office 2016. Служби віддалених робочих столів раніше назвили службами терміналів.
  