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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571292"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b83da-102">Не вдалося видалити елементи</span><span class="sxs-lookup"><span data-stu-id="b83da-102">Unable to delete items</span></span>

<span data-ttu-id="b83da-103">Політика збереження може спричинити це, потрібно або вимкнути або виключити відповідні утримання, що спричиняє цю проблему.</span><span class="sxs-lookup"><span data-stu-id="b83da-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="b83da-104">Після того, як буде видалено політику збереження або утримання, може тривати до 24 годин, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="b83da-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="b83da-105">Переконайтеся, що на елементі не існує настроювання [політики збереження](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="b83da-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="b83da-106">Можливо, на сайті Перевищено граничний обсяг сховища, збільшення [квоти сайту](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) та видалення елемента.</span><span class="sxs-lookup"><span data-stu-id="b83da-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="b83da-107">Переконайтеся, що елемент не [витягнуто](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) іншому користувачу.</span><span class="sxs-lookup"><span data-stu-id="b83da-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="b83da-108">Нарешті, адміністратори можуть використовувати [SharePoint шаблонів і практик](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (ПНП), яка містить бібліотеку команд PowerShell, які дозволяють виконувати складні дії керування, наприклад, примусове видалення впертих елементів.</span><span class="sxs-lookup"><span data-stu-id="b83da-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="b83da-109">Видалити ПНП файл</span><span class="sxs-lookup"><span data-stu-id="b83da-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b83da-110">Видалити ПНП папку</span><span class="sxs-lookup"><span data-stu-id="b83da-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b83da-111">Видалити ПНП елемент списку</span><span class="sxs-lookup"><span data-stu-id="b83da-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b83da-112">Видалити ПНП список</span><span class="sxs-lookup"><span data-stu-id="b83da-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b83da-113">Видалення поля «ПНП» (стовпець)</span><span class="sxs-lookup"><span data-stu-id="b83da-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)