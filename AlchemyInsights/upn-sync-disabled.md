---
title: Синхронізація за допомогою UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749535"
---
# <a name="upn-sync-disabled"></a>Синхронізація за допомогою UPN

Якщо ви почали синхронізуватися в Azure AD до 30 березня 2016, запустіть цей командлет, щоб увімкнути м'який засіб для організації, виконавши такі дії:
  
 **Set-Msololrsyncфункція – функція EnableSoftMatchOnUpn-увімкнути $True**
  
Для організацій, які почали синхронізуватися з Azure AD на або після 30 березня 2016, автоматично вмикається відповідність.
  
Щоб дізнатися більше про те, як ввімкнути м'яку відповідність за допомогою функції UPN та інших функцій синхронізації, ознайомтеся з [функціями служби синхронізації Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

