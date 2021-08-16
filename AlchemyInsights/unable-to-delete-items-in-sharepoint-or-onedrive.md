---
title: Не вдається видалити елементи в SharePoint або OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038538"
---
# <a name="unable-to-delete-items"></a>Не вдається видалити елементи

- Політики збереження можуть спричинити це, потрібно вимкнути або виключити відповідне утримання, яке спричиняє цю проблему. Коли політику збереження або утримання буде видалено, зміни наберуть сили протягом 24 годин. Переконайтеся, що для елемента немає [налаштування](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) політики збереження.

- Можливо, перевищено граничне обсяг сховища сайту, збільште квоту сайту [та](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) видаліть елемент.

- Переконайтеся, що елемент не [взяв на редагування](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) для іншого користувача.

- Нарешті, адміністратори можуть використовувати [SharePoint шаблони](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) та практики (PNP), яка містить бібліотеку команд PowerShell, яка дає змогу виконувати складні дії керування, наприклад примусово видаляти неузахистані елементи.
- [Видалення PNP-файлу](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Видалити папку PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Видалити елемент списку PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Вилучення списку PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Видалення поля PNP (стовпця)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)