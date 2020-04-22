---
title: Сертифікат ADFS Федерації закінчується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710428"
---
# <a name="adfs-federation-certificate-expiring"></a>Сертифікат ADFS Федерації закінчується

Щоб вирішити цю проблему, виконайте такі дії:
  
1. Інсталюйте модуль Microsoft Azure Active Directory для оболонки Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Для цього перейдіть до [керування AZURE AD за допомогою оболонки Windows PowerShell](https://aka.ms/aadposh).

2. Виконайте дії, описані в "сценарій 1: AD FS маркер підпису сертифікат минув" розділу ["сталася помилка доступу до сайту" повідомлення про помилку з AD FS, коли федеративного користувача входить до Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Виконайте дії, описані в [розділі оновлення або відновлення параметрів федеративного домену, у Microsoft, Azure або InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Щоб дізнатися більше про оновлення об'єднання сертифікатів, див., [оновлення об'єднання сертифікати для Microsoft 365 і Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
