---
title: Один із сертифікати служби локальної Федерації закінчується
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785324"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Один із сертифікати служби локальної Федерації закінчується

Щоб вирішити цю проблему, виконайте такі дії:
  
- Інсталюйте модуль Microsoft Azure Active Directory для оболонки Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Для цього перейдіть до [Azure Active Directory PowerShell для графа](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Виконайте дії, описані в "сценарій 1: AD FS маркер підпису сертифікат минув" розділу ["сталася помилка доступу до сайту" повідомлення про помилку з AD FS, коли федеративного користувача входить до Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Виконайте дії, [як оновити або відновити параметри федеративного домену, у Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Щоб отримати додаткові відомості про оновлення об'єднання сертифікатів, див [оновлення сертифікатів O365 і AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

