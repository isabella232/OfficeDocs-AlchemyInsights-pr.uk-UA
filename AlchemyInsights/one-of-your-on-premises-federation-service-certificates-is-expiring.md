---
title: Завершується одна з сертифікатів служби локальної Федерації
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673518"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Завершується одна з сертифікатів служби локальної Федерації

Щоб вирішити цю проблему, виконайте наведені нижче дії.
  
- Інсталюйте модуль Microsoft Azure Active Directory для оболонки Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Щоб виконати цю дію, перейдіть до [PowerShell для графа "Azure Active Directory](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) "
    
- Виконайте кроки, описані в розділі "сценарії 1: маркер AD FS", термін дії якого завершився " [Помилка під час доступу до сайту" з AD FS, коли Федеративний користувач підписує в Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Виконайте вказівки з [оновлення або відновлення параметрів федеративного домену в Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Докладні відомості про сертифікати Федерації поновлення наведено в статті [оновлення сертифіката для O365 і Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

