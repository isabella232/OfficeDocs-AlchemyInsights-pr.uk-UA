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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952990"
---
# <a name="adfs-federation-certificate-expiring"></a>Термін дії сертифіката федерації ADFS завершується

Щоб вирішити цю проблему, виконайте такі дії:
  
1. Інсталюйте Microsoft Azure Active Directory модуль Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Для цього перейдіть до керування [Azure AD за допомогою Windows PowerShell](https://aka.ms/aadposh).

2. Виконайте кроки, описані в розділі "Сценарій 1. Термін дії сертифіката підпису маркера AD FS завершився" статті Помилка "Сталася помилка доступу до сайту" з AD FS, коли федеративний користувач увійшов у [Microsoft 365, Azure або Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Виконайте кроки, описані в статті Оновлення або відновлення параметрів федеративного домену [в Microsoft, Azure або Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Докладні відомості про поновлення сертифікатів федерації див. в статтях Поновлення сертифікатів федерації для [Microsoft 365 та Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
