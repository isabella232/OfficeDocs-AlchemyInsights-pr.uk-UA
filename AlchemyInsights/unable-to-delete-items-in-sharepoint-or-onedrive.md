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
# <a name="unable-to-delete-items"></a><span data-ttu-id="24dac-102">Не вдалося видалити елементи</span><span class="sxs-lookup"><span data-stu-id="24dac-102">Unable to delete items</span></span>

<span data-ttu-id="24dac-103">З питань видалення елементів?</span><span class="sxs-lookup"><span data-stu-id="24dac-103">Having issues deleting items?</span></span>

- <span data-ttu-id="24dac-104">Завжди переконайтесь, що у вас є [відповідні дозволи](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) на Видалити об'єкт або мають [адміністратор колекції сайтів](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) спроба видалити елемент.</span><span class="sxs-lookup"><span data-stu-id="24dac-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="24dac-105">Переконайтеся, що це не [політика збереження](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) установки на елементі.</span><span class="sxs-lookup"><span data-stu-id="24dac-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="24dac-106">Переконайтеся, елемент не [взяв на редагування](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) інший користувач.</span><span class="sxs-lookup"><span data-stu-id="24dac-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="24dac-107">Нарешті, адміністратори можуть використовувати [SharePoint візерунки і практики](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) які містить бібліотека PowerShell команди, які дозволяють виконувати складні управління дії таких як змусити видалення впертий елементів.</span><span class="sxs-lookup"><span data-stu-id="24dac-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="24dac-108">Видалити PNP-файл</span><span class="sxs-lookup"><span data-stu-id="24dac-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="24dac-109">Видалити PNP папки</span><span class="sxs-lookup"><span data-stu-id="24dac-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="24dac-110">Видалення елемента списку PNP</span><span class="sxs-lookup"><span data-stu-id="24dac-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="24dac-111">Видалити PNP список</span><span class="sxs-lookup"><span data-stu-id="24dac-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="24dac-112">Видалити PNP поля (стовпця)</span><span class="sxs-lookup"><span data-stu-id="24dac-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)