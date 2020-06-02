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
# <a name="fix-dkim-setup-issues"></a>Вирішення проблем із налаштуванням DKIM

Якщо виникають проблеми, які дозволяють DKIM для настроюваного домену, виконайте такі дії:

- Більшість проблем з настройки DKIM пов'язані з неправильні записи DNS. Переконайтеся, що запис DKIM CNAME (**не** запис txt) відформатовано правильно. Докладніші відомості наведено в цій [статті](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Після створення або оновлення DKIM записів DNS у службі розміщення DNS для вашого домену (як правило, ваш домен реєстратора), зачекайте, доки записи DNS для розповсюдження.

- Якщо не вдається створити записи DNS DKIM в центрі адміністрування, можна замінити на \<CustomDomain\> власний домен (наприклад, contoso.com) і запустити цю команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
