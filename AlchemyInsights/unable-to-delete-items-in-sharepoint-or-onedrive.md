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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806132"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b3681-102">Не вдається видалити елементи</span><span class="sxs-lookup"><span data-stu-id="b3681-102">Unable to delete items</span></span>

<span data-ttu-id="b3681-103">Політики збереження можуть спричиняти цю проблему, щоб вимкнути або виключити відповідний запит.</span><span class="sxs-lookup"><span data-stu-id="b3681-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="b3681-104">Після видалення політики збереження або утримання може знадобитися до 24 годин, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="b3681-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="b3681-105">Переконайтеся, що для елемента немає настроювання [політики збереження](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="b3681-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="b3681-106">Можливо, на сайті Перевищено граничний обсяг сховища, збільшити [квоту сайту](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) та видалити елемент.</span><span class="sxs-lookup"><span data-stu-id="b3681-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="b3681-107">Переконайтеся, що елемент не [витягнуто](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) іншим користувачем.</span><span class="sxs-lookup"><span data-stu-id="b3681-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="b3681-108">Нарешті, адміністратори можуть використовувати [шаблони SharePoint і практику](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), що містить бібліотеку з командами PowerShell, які дають змогу виконувати складні дії з керування, наприклад примусово видаляти вперті елементи.</span><span class="sxs-lookup"><span data-stu-id="b3681-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="b3681-109">Видалення файлу PNP</span><span class="sxs-lookup"><span data-stu-id="b3681-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b3681-110">Видалення папки PNP</span><span class="sxs-lookup"><span data-stu-id="b3681-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b3681-111">Видалення елемента списку PNP</span><span class="sxs-lookup"><span data-stu-id="b3681-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b3681-112">Видалення списку PNP</span><span class="sxs-lookup"><span data-stu-id="b3681-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b3681-113">Видалення поля PNP (стовпець)</span><span class="sxs-lookup"><span data-stu-id="b3681-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)