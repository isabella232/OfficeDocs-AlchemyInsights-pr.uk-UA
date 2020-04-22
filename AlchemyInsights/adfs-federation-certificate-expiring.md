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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="cfd3c-102">Сертифікат ADFS Федерації закінчується</span><span class="sxs-lookup"><span data-stu-id="cfd3c-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="cfd3c-103">Щоб вирішити цю проблему, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="cfd3c-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="cfd3c-104">Інсталюйте модуль Microsoft Azure Active Directory для оболонки Windows PowerShell на комп'ютері (якщо модуль ще не інстальовано).</span><span class="sxs-lookup"><span data-stu-id="cfd3c-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="cfd3c-105">Для цього перейдіть до [керування AZURE AD за допомогою оболонки Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="cfd3c-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="cfd3c-106">Виконайте дії, описані в "сценарій 1: AD FS маркер підпису сертифікат минув" розділу ["сталася помилка доступу до сайту" повідомлення про помилку з AD FS, коли федеративного користувача входить до Microsoft 365, Azure або InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="cfd3c-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="cfd3c-107">Виконайте дії, описані в [розділі оновлення або відновлення параметрів федеративного домену, у Microsoft, Azure або InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="cfd3c-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="cfd3c-108">Щоб дізнатися більше про оновлення об'єднання сертифікатів, див., [оновлення об'єднання сертифікати для Microsoft 365 і Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="cfd3c-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
