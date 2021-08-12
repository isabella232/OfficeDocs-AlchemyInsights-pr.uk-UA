---
title: Підключення до модуля MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974696"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MsCommerce потребує облікового запису адміністратора компанії або облікового запису адміністратора з виставлення рахунків

Модуль MSCommerce потребує облікового запису з правами адміністратора компанії або облікового запису. Якщо з'являється наведене нижче повідомлення про помилку, потрібно повторно підключити інший обліковий запис.

*ErrorMessage – віддалений сервер повернув помилку: (403) Заборонено. ErrorDetails – at C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Не вдалося повторити ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Якщо ваш обліковий запис не має прав адміністратора компанії або облікового запису, зверніться до ІТ-адміністратора.
