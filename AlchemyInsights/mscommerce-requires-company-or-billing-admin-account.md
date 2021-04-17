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
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829757"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MsCommerce потребує облікового запису адміністратора компанії або облікового запису адміністратора з виставлення рахунків

Модуль MSCommerce потребує облікового запису з правами адміністратора компанії або облікового запису. Якщо з'являється наведене нижче повідомлення про помилку, потрібно повторно підключити інший обліковий запис.

*ErrorMessage – віддалений сервер повернув помилку: (403) Заборонено. ErrorDetails – at C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Не вдалося повторити ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Якщо ваш обліковий запис не має прав адміністратора компанії або облікового запису, зверніться до ІТ-адміністратора.
