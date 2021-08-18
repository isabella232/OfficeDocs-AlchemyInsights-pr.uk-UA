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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316707"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Помилка під час активації Office 2013 у службах віддалених робочих столів

Якщо під час активації пакета Office 2013 у розгортань служб віддалених робочих столів (RDS) з'являється повідомлення про помилку, редагуючи реєстр, можна активувати ADAL.
  
|**Розділ реєстру**|**Тип**|**Значення**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Докладні відомості див. в [сторінці Активація сучасної автентифікації Office 2013 на Windows пристроях.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Примітка.** ADAL активовано за замовчуванням у Програми Microsoft 365 для підприємств 2016 Office. Служби віддалених робочих столів (RDS) раніше назвували службами терміналів.
  