---
title: Не вдалося видалити елементи в SharePoint або OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057796"
---
# <a name="unable-to-delete-items"></a>Не вдалося видалити елементи

З питань видалення елементів?

- Завжди переконайтесь, що у вас є [відповідні дозволи](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) на Видалити об'єкт або мають [адміністратор колекції сайтів](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) спроба видалити елемент.

- Переконайтеся, що це не [політика збереження](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) установки на елементі.

- Переконайтеся, елемент не [взяв на редагування](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) інший користувач.

- Нарешті, адміністратори можуть використовувати [SharePoint візерунки і практики](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) які містить бібліотека PowerShell команди, які дозволяють виконувати складні управління дії таких як змусити видалення впертий елементів. 
- [Видалити PNP-файл](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Видалити PNP папки](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Видалення елемента списку PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Видалити PNP список](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Видалити PNP поля (стовпця)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)