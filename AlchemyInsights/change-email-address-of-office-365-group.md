---
title: Змінення адреси електронної пошти групи Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580678"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="39e37-102">Змінення адреси електронної пошти групи Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="39e37-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="39e37-103">Можна змінити адресу електронної пошти групи Microsoft 365 за допомогою Центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="39e37-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="39e37-104">Просто виберіть групу і виберіть @edit адресу електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="39e37-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="39e37-105">Ви також можете використовувати наступні команди EXO PowerShell для зміни основна адреса SMTP групи Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="39e37-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="39e37-106">Набір-UnifiedGroup <Group Name> -первинний, адресадреса<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="39e37-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="39e37-107">Приклад:</span><span class="sxs-lookup"><span data-stu-id="39e37-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
