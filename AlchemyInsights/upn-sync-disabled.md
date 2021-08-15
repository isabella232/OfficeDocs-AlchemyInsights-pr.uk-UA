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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038133"
---
# <a name="upn-sync-disabled"></a>Синхронізацію UPN вимкнуто

Якщо синхронізація з Azure AD почалася до 30 березня 2016 р., запустіть цей командлет Azure AD PowerShell, щоб активувати лише м'які збіги UPN для організації:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
М'які збіги upN автоматично активуються для організацій, які почали синхронізуватися з Azure AD 30 березня 2016 р. або після 30 березня 2016 р.
  
Докладні відомості про ввімкнення м'якого збігу в UPN та інші функції синхронізації див. в Підключення [Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

