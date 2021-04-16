---
title: Термін дії одного з локальних сертифікатів служби об'єднання завершується
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810073"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Термін дії одного з локальних сертифікатів служби об'єднання завершується

Щоб вирішити цю проблему, виконайте такі дії:
  
- Інсталюйте модуль Microsoft Azure Active Directory для Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Для цього перейдіть до [Azure Active Directory PowerShell для Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Виконайте кроки, описані в розділі "Сценарій 1. Термін дії сертифіката підпису маркера AD FS завершився" статті Помилка "Сталася помилка доступу до сайту" з AD FS, коли федеративний користувач увійшов у [Microsoft 365, Azure або Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Виконайте вказівки з оновлення або відновлення параметрів федеративного домену в [Microsoft 365, Azure або Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Докладні відомості про поновлення сертифікатів федерації див. в відомостях про поновлення [сертифікатів для O365 і Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

