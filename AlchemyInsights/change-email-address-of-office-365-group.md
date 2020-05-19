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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283265"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="8b5f3-102">Змінення адреси електронної пошти групи Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8b5f3-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="8b5f3-103">Можна змінити адресу електронної пошти групи Microsoft 365 за допомогою Центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="8b5f3-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="8b5f3-104">Просто виберіть групу і виберіть @edit адресу електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="8b5f3-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="8b5f3-105">Ви також можете використовувати наступні команди EXO PowerShell для зміни основна адреса SMTP групи Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="8b5f3-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="8b5f3-106">Набір-UnifiedGroup <Group Name> -первинний, адресадреса<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="8b5f3-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="8b5f3-107">Приклад:</span><span class="sxs-lookup"><span data-stu-id="8b5f3-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
