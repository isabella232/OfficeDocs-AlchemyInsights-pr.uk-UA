---
title: Розташування даних
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627867"
---
# <a name="data-location"></a>Розташування даних

Ви можете переглянути розташування вашого клієнта Office 365 в центрі адміністрування або шляхом підключення до Exchange Online через PowerShell.


**Центр адміністрування:**
1. Увійдіть в [Центр адміністрування](https://admin.microsoft.com/Adminportal/Home).
2. Виберіть **** > **профіль організації**настройки.
3. У розділі **розташування даних**виберіть **переглянути деталі**.


**Powershell:**
1. Підключення до Exchange Online за допомогою оболонки Windows PowerShell.
2. Виконати командлет [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) для відображення списку властивостей вашого клієнта. 
3. Подивіться на власність Організаціїid.

Якщо у вас є дані розташування для EXO і спо, ви можете визначити розташування даних для інших послуг, які ви можете використовувати, [де ваші дані знаходяться](https://products.office.com/where-is-your-data-located).