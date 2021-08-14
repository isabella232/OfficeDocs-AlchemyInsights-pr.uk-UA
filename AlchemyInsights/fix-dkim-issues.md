---
title: Вирішення проблем із налаштуванням DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945952"
---
# <a name="fix-dkim-setup-issues"></a>Вирішення проблем із налаштуванням DKIM

Якщо у вас виникають проблеми з увімкненням DKIM для настроюваного домену, виконайте такі дії:

- Більшість проблем із настроюванням DKIM пов'язані з неправильними записами DNS. Переконайтеся, що запис CNAME DKIM **(не** запис TXT) відформатовано належним чином. Докладні відомості див. в цій [статті](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Створиивши або оновивши записи DNS DKIM у службі розміщення DNS для свого домену (зазвичай це ваш реєстратор доменів), зачекайте, доки записи DNS розміщаться.

- Якщо не вдається створити записи DNS DKIM у Центрі адміністрування, можна замінити їх на настроюваний домен (наприклад, contoso.com) і виконати цю команду в \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
