---
title: Активувати аудит поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500303"
---
# <a name="enable-mailbox-auditing"></a>Активувати аудит поштової скриньки

Щоб активувати аудит поштової скриньки для одного користувача або всією установою наведені нижче команди cmdlet має бути запущено з віддаленої оболонки живлення:
  
 **Одного користувача**
  
Set-Mailbox - ідентичності "Джейн Доу" - AuditEnabled $true
  
 Organization
  
Get-Mailbox - ResultSize необмежений - фільтрувати {"UserMailbox", RecipientTypeDetails - eq} | Set-Mailbox - AuditEnabled $true
  
Додаткові відомості
  

