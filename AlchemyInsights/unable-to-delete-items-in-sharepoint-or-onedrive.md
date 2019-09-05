---
title: Не вдалося видалити елементи в SharePoint або OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748597"
---
# <a name="unable-to-delete-items"></a>Не вдалося видалити елементи

Виникли проблеми з видаленням елементів SharePoint?

- Завжди переконайтеся, що у вас є [відповідні дозволи](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) на видалення елемента або є спроба [адміністратор колекції сайтів](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) видалити елемент.

- Переконайтеся, що на елементі не існує настроювання [політики збереження](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

- Переконайтеся, що елемент не [витягнуто](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) іншому користувачу.

- Нарешті, адміністратори можуть використовувати [SharePoint шаблонів і практик](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (ПНП), яка містить бібліотеку команд PowerShell, які дозволяють виконувати складні дії керування, наприклад, примусове видалення впертих елементів.
- [Видалити ПНП файл](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Видалити ПНП папку](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Видалити ПНП елемент списку](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Видалити ПНП список](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Видалення поля «ПНП» (стовпець)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)