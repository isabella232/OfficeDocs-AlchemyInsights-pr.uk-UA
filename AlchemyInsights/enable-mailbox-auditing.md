---
title: Увімкнути аудит поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736274"
---
# <a name="enable-mailbox-auditing"></a>Увімкнути аудит поштової скриньки

Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, потрібно запустити такі командлети з віддаленої оболонки живлення:
  
 **Одного користувача**
  
Set-поштова скринька-Identity "Джейн Доу"-аудита $true
  
 **Організації**
  
Get-поштова скринька-розмір необмежений фільтр {RecipientTypeDetails-EQ "UserMailbox скринька"} | Набір-поштова скринька-можливість аудита $true
  
[Дізнатися більше](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

