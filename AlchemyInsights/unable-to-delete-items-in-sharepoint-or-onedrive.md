---
title: Не вдається видалити елементи в службі SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019604"
---
# <a name="unable-to-delete-items"></a>Не вдається видалити елементи

- Політики збереження можуть спричиняти цю проблему, щоб вимкнути або виключити відповідний запит. Після видалення політики збереження або утримання може знадобитися до 24 годин, щоб зміни набрали сили. Переконайтеся, що для елемента немає настроювання [політики збереження](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .

- Можливо, на сайті Перевищено граничний обсяг сховища, збільшити [квоту сайту](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) та видалити елемент.

- Переконайтеся, що елемент не [витягнуто](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) іншим користувачем.

- Нарешті, адміністратори можуть використовувати [шаблони SharePoint і практику](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), що містить бібліотеку з командами PowerShell, які дають змогу виконувати складні дії з керування, наприклад примусово видаляти вперті елементи.
- [Видалення файлу PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Видалення папки PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Видалення елемента списку PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Видалення списку PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Видалення поля PNP (стовпець)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)