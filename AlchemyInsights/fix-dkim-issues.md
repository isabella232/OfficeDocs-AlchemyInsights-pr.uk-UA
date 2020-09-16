---
title: Вирішення проблем із інсталяцією DKIM
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744971"
---
# <a name="fix-dkim-setup-issues"></a>Вирішення проблем із інсталяцією DKIM

Якщо у вас виникли проблеми, які дають змогу DKIM для свого настроюваного домену, виконайте наведені нижче дії.

- Більшість проблем із інсталяцією DKIM пов'язано з неправильними записами DNS. Переконайтеся, що запис CNAME DKIM (**не** запис txt) відформатовано правильно. Щоб отримати докладніші відомості, ознайомтеся з цією [темою](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Створивши або оновіть записи DNS DKIM у службі розміщення DNS для домену (зазвичай, реєстратора доменів), зачекайте, доки не буде поширюватися записи DNS.

- Якщо ви не можете створити записи DNS DKIM в центрі адміністрування, можна замінити його \<CustomDomain\> настроюваним доменом (наприклад, contoso.com) і виконати цю команду в [службі Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
