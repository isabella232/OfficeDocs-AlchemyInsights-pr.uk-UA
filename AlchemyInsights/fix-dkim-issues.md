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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717583"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="9d1ba-102">Вирішення проблем із налаштуванням DKIM</span><span class="sxs-lookup"><span data-stu-id="9d1ba-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="9d1ba-103">Якщо виникають проблеми, які дозволяють DKIM для настроюваного домену, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="9d1ba-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="9d1ba-104">Більшість проблем з настройки DKIM пов'язані з неправильні записи DNS.</span><span class="sxs-lookup"><span data-stu-id="9d1ba-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="9d1ba-105">Переконайтеся, що запис DKIM CNAME (**не** запис txt) відформатовано правильно.</span><span class="sxs-lookup"><span data-stu-id="9d1ba-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="9d1ba-106">Докладніші відомості наведено в цій [статті](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9d1ba-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="9d1ba-107">Після створення або оновлення DKIM записів DNS у службі розміщення DNS для вашого домену (як правило, ваш домен реєстратора), зачекайте, доки записи DNS для розповсюдження.</span><span class="sxs-lookup"><span data-stu-id="9d1ba-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="9d1ba-108">Якщо не вдається створити записи DNS DKIM в центрі адміністрування, \<можна замінити\> настроюваний домен на власний домен (наприклад, contoso.com) і запустити цю команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`</span><span class="sxs-lookup"><span data-stu-id="9d1ba-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
