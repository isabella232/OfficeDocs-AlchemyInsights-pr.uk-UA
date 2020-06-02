---
title: Увімкнути аудит поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506975"
---
# <a name="enable-mailbox-auditing"></a>Увімкнути аудит поштової скриньки

Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, потрібно запустити такі командлети з віддаленої оболонки живлення:
  
 **Одного користувача**
  
Set-поштова скринька-Identity "Джейн Доу"-аудита $true
  
 **Організації**
  
Get-поштова скринька-розмір необмежений фільтр {RecipientTypeDetails-EQ "UserMailbox скринька"} | Набір-поштова скринька-можливість аудита $true
  
[Дізнатися більше](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

