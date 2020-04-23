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
# <a name="fix-dkim-setup-issues"></a>Вирішення проблем із налаштуванням DKIM

Якщо виникають проблеми, які дозволяють DKIM для настроюваного домену, виконайте такі дії:

- Більшість проблем з настройки DKIM пов'язані з неправильні записи DNS. Переконайтеся, що запис DKIM CNAME (**не** запис txt) відформатовано правильно. Докладніші відомості наведено в цій [статті](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Після створення або оновлення DKIM записів DNS у службі розміщення DNS для вашого домену (як правило, ваш домен реєстратора), зачекайте, доки записи DNS для розповсюдження.

- Якщо не вдається створити записи DNS DKIM в центрі адміністрування, \<можна замінити\> настроюваний домен на власний домен (наприклад, contoso.com) і запустити цю команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
