---
title: Вирішення проблем із налаштуванням DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506795"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="6dc15-102">Вирішення проблем із налаштуванням DKIM</span><span class="sxs-lookup"><span data-stu-id="6dc15-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="6dc15-103">Якщо виникають проблеми, які дозволяють DKIM для настроюваного домену, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="6dc15-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="6dc15-104">Більшість проблем з настройки DKIM пов'язані з неправильні записи DNS.</span><span class="sxs-lookup"><span data-stu-id="6dc15-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="6dc15-105">Переконайтеся, що запис DKIM CNAME (**не** запис txt) відформатовано правильно.</span><span class="sxs-lookup"><span data-stu-id="6dc15-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6dc15-106">Докладніші відомості наведено в цій [статті](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="6dc15-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="6dc15-107">Після створення або оновлення DKIM записів DNS у службі розміщення DNS для вашого домену (як правило, ваш домен реєстратора), зачекайте, доки записи DNS для розповсюдження.</span><span class="sxs-lookup"><span data-stu-id="6dc15-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="6dc15-108">Якщо не вдається створити записи DNS DKIM в центрі адміністрування, можна замінити на \<CustomDomain\> власний домен (наприклад, contoso.com) і запустити цю команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="6dc15-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
