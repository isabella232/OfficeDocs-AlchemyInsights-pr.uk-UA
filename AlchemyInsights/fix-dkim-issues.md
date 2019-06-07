---
title: Виправлення неполадок інсталяції DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765527"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="8c567-102">Виправлення неполадок інсталяції DKIM</span><span class="sxs-lookup"><span data-stu-id="8c567-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="8c567-103">Якщо у вас виникли питання, що дозволяє DKIM вашого користувача домену, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="8c567-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="8c567-104">Більшість DKIM установки питань пов'язаних з неправильні записи DNS.</span><span class="sxs-lookup"><span data-stu-id="8c567-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="8c567-105">Перевірте, чи правильно відформатовано на DKIM запис CNAME (**не** запис TXT).</span><span class="sxs-lookup"><span data-stu-id="8c567-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="8c567-106">Докладніше перегляньте цю [тему](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="8c567-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="8c567-107">Після створення або оновлення записи DKIM DNS в до служби розміщення DNS для свого домену (як правило, ваш Реєстратор домену), зачекайте, поки записи DNS для поширення.</span><span class="sxs-lookup"><span data-stu-id="8c567-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="8c567-108">Якщо неможливо створити DKIM DNS записів центру адміністрування, можна замінити \<CustomDomain\> з вашого користувача домену (наприклад, contoso.com) і виконайте цю команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="8c567-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
