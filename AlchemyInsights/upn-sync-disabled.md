---
title: Синхронізацію UPN вимкнуто
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782172"
---
# <a name="upn-sync-disabled"></a>Синхронізацію UPN вимкнуто

Якщо синхронізація з Azure AD почалася до 30 березня 2016 р., запустіть цей командлет Azure AD PowerShell, щоб активувати лише м'які збіги UPN для організації:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
М'які збіги upN автоматично активуються для організацій, які почали синхронізуватися з Azure AD 30 березня 2016 р. або після 30 березня 2016 р.
  
Докладні відомості про те, як ввімкнути м'які збіги в UPN та інші функції синхронізації, див. в статтях [Функції служби синхронізації Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

