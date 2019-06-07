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
# <a name="fix-dkim-setup-issues"></a>Виправлення неполадок інсталяції DKIM

Якщо у вас виникли питання, що дозволяє DKIM вашого користувача домену, виконайте такі дії:

- Більшість DKIM установки питань пов'язаних з неправильні записи DNS. Перевірте, чи правильно відформатовано на DKIM запис CNAME (**не** запис TXT). Докладніше перегляньте цю [тему](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Після створення або оновлення записи DKIM DNS в до служби розміщення DNS для свого домену (як правило, ваш Реєстратор домену), зачекайте, поки записи DNS для поширення.

- Якщо неможливо створити DKIM DNS записів центру адміністрування, можна замінити \<CustomDomain\> з вашого користувача домену (наприклад, contoso.com) і виконайте цю команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
