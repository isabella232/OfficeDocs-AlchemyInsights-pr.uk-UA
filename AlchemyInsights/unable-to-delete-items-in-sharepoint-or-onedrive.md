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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748597"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="60db3-102">Не вдалося видалити елементи</span><span class="sxs-lookup"><span data-stu-id="60db3-102">Unable to delete items</span></span>

<span data-ttu-id="60db3-103">Виникли проблеми з видаленням елементів SharePoint?</span><span class="sxs-lookup"><span data-stu-id="60db3-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="60db3-104">Завжди переконайтеся, що у вас є [відповідні дозволи](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) на видалення елемента або є спроба [адміністратор колекції сайтів](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) видалити елемент.</span><span class="sxs-lookup"><span data-stu-id="60db3-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="60db3-105">Переконайтеся, що на елементі не існує настроювання [політики збереження](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="60db3-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="60db3-106">Переконайтеся, що елемент не [витягнуто](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) іншому користувачу.</span><span class="sxs-lookup"><span data-stu-id="60db3-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="60db3-107">Нарешті, адміністратори можуть використовувати [SharePoint шаблонів і практик](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (ПНП), яка містить бібліотеку команд PowerShell, які дозволяють виконувати складні дії керування, наприклад, примусове видалення впертих елементів.</span><span class="sxs-lookup"><span data-stu-id="60db3-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="60db3-108">Видалити ПНП файл</span><span class="sxs-lookup"><span data-stu-id="60db3-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="60db3-109">Видалити ПНП папку</span><span class="sxs-lookup"><span data-stu-id="60db3-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="60db3-110">Видалити ПНП елемент списку</span><span class="sxs-lookup"><span data-stu-id="60db3-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="60db3-111">Видалити ПНП список</span><span class="sxs-lookup"><span data-stu-id="60db3-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="60db3-112">Видалення поля «ПНП» (стовпець)</span><span class="sxs-lookup"><span data-stu-id="60db3-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)