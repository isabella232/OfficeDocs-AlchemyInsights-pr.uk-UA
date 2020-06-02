---
title: Не вдалося видалити елементи в SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511997"
---
# <a name="unable-to-delete-items"></a>Не вдалося видалити елементи

Політика збереження може спричинити це, потрібно або вимкнути або виключити відповідні утримання, що спричиняє цю проблему. Після того, як буде видалено політику збереження або утримання, може тривати до 24 годин, щоб зміни набрали сили. Переконайтеся, що на елементі не існує настроювання [політики збереження](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .

Можливо, на сайті Перевищено граничний обсяг сховища, збільшення [квоти сайту](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) та видалення елемента.

Переконайтеся, що елемент не [витягнуто](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) іншому користувачу.

Нарешті, адміністратори можуть використовувати [SharePoint шаблонів і практик](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (ПНП), яка містить бібліотеку команд PowerShell, які дозволяють виконувати складні дії керування, наприклад, примусове видалення впертих елементів.
- [Видалити ПНП файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Видалити ПНП папку](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Видалити ПНП елемент списку](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Видалити ПНП список](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Видалення поля «ПНП» (стовпець)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)