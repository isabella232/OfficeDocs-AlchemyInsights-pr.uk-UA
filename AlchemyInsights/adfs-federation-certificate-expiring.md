---
title: Сертифікат ADFS Федерації закінчується
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
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737210"
---
# <a name="adfs-federation-certificate-expiring"></a>Сертифікат ADFS Федерації закінчується

Щоб вирішити цю проблему, виконайте такі дії:
  
1. Інсталюйте модуль Microsoft Azure Active Directory для оболонки Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано). Для цього перейдіть до [керування AZURE AD за допомогою оболонки Windows PowerShell](https://aka.ms/aadposh).

2. Виконайте дії, описані в "сценарій 1: AD FS маркер підпису сертифікат минув" розділу ["сталася помилка доступу до сайту" повідомлення про помилку з AD FS, коли федеративного користувача входить до Office 365, Azure або InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Виконайте дії, описані в [розділі оновлення або відновлення параметрів федеративного домену в Office 365, Azure або InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Щоб дізнатися більше про оновлення об'єднання сертифікатів, див., [оновлення об'єднання сертифікати для Office 365 і Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
