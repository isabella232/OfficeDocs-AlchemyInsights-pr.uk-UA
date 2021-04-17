---
title: Термін дії сертифіката федерації ADFS завершується
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821972"
---
# <a name="adfs-federation-certificate-expiring"></a>Термін дії сертифіката федерації ADFS завершується

Щоб вирішити цю проблему, виконайте такі дії:
  
1. Інсталюйте модуль Microsoft Azure Active Directory для Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Для цього перейдіть до керування [Azure AD за допомогою Windows PowerShell.](https://aka.ms/aadposh)

2. Виконайте кроки, описані в розділі "Сценарій 1. Термін дії сертифіката підпису маркера AD FS завершився" статті Помилка "Сталася помилка доступу до сайту" з AD FS, коли федеративний користувач увійшов у [Microsoft 365, Azure або Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Виконайте кроки, описані в статті Оновлення або відновлення параметрів федеративного домену [в Microsoft, Azure або Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Докладні відомості про поновлення сертифікатів федерації див. в статтях Поновлення сертифікатів федерації [для Microsoft 365 і Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
