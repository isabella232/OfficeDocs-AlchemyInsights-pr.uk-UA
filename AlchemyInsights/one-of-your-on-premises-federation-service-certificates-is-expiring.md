---
title: Один з ваших локальні служби Федерації сертифікатів закінчується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543730"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Один з ваших локальні служби Федерації сертифікатів закінчується

Щоб вирішити цю проблему, виконайте такі дії:
  
- Встановити на Microsoft Azure Active Directory модуль для Windows PowerShell на комп'ютер (якщо модуль не встановлений). Для цього перейдіть на [Azure Active Directory PowerShell графіка](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Виконайте дії, описані в на "сценарій 1: AD FS маркер підписання сертифіката минув" розділ [«Виникла проблема доступу до сайту» помилка з AD FS коли федеративного користувач входить до Office 365, Azure або Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Дотримуйтесь інструкцій у t[як оновити або відновити параметри інтегрований домен у службі Office 365, Azure або Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Щоб отримати додаткові відомості про поновлення Федерації сертифікатів див [сертифіката відновлення для O365 і блакитні оголошення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

