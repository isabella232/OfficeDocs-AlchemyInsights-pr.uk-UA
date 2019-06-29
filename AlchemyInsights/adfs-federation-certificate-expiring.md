---
title: ADFS Федерація сертифікат закінчується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: b014e350d5f6f1a61feb223e3d3fd0a1f56f5872
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357986"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Федерація сертифікат закінчується

Щоб вирішити цю проблему, виконайте такі дії:
  
1. Встановити на Microsoft Azure Active Directory модуль для Windows PowerShell на комп'ютер (якщо модуль не встановлений). Для цього, перейти до [керування блакитні оголошення за допомогою Windows PowerShell](https://aka.ms/aadposh).

2. Виконайте дії, описані в на "сценарій 1: AD FS маркер підписання сертифіката минув" розділ [«Виникла проблема доступу до сайту» помилка з AD FS коли федеративного користувач входить до Office 365, Azure або Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Виконайте [як оновити або відновити параметри інтегрований домен у службі Office 365, Azure або Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Щоб дізнатися більше про поновлення Федерації сертифікати, побачити [Renew Федерації сертифікати для Office 365 і Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
