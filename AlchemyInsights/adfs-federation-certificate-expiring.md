---
title: Термін дії сертифіката Федерації ADFS завершується
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686777"
---
# <a name="adfs-federation-certificate-expiring"></a>Термін дії сертифіката Федерації ADFS завершується

Щоб вирішити цю проблему, виконайте наведені нижче дії.
  
1. Інсталюйте модуль Microsoft Azure Active Directory для оболонки Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Щоб зробити це, перейдіть на сторінку [керування Azure AD за допомогою оболонки Windows PowerShell](https://aka.ms/aadposh).

2. Виконайте кроки, описані в розділі "сценарії 1: маркер AD FS", термін дії якого завершився " [Помилка під час доступу до сайту" з AD FS, коли Федеративний користувач підписує в Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Виконайте кроки, описані в статті [оновлення або відновлення параметрів федеративного домену в Microsoft, Azure або InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Докладні відомості про сертифікати Федерації поновлення наведено в статті [поновлення сертифікатів Федерації для служби Microsoft 365 і "Лазурний" (Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)).
