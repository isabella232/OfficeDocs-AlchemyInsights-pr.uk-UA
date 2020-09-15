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
description: Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 у розгортаннях служб віддалених робочих столів (RDS), радимо ввімкнути параметр ADAL, змінивши реєстр.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709208"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Помилка під час активації Office 2013 на віддалених настільних службах

Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 у розгортаннях служб віддалених робочих столів (RDS), радимо ввімкнути параметр ADAL, змінивши реєстр.
  
|**Розділ реєстру**|**Введіть**|**Значення**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Докладні відомості наведено в статті [Увімкнення сучасної автентифікації для Office 2013 на пристроях з ОС Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Служба ADAL ввімкнена за замовчуванням у програмах Microsoft 365 для підприємств і Office 2016. Служби віддалених настільних комп'ютерів (RDS) раніше були іменованими службами терміналів.
  