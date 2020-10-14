---
title: Спільна папка "Надіслати як пошта" в програмі EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462077"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="def13-102">Спільна папка "пошта" з підтримкою SendAs</span><span class="sxs-lookup"><span data-stu-id="def13-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="def13-103">У наведеному нижче прикладі призначається дозвіл "Надіслати як" для спільної папки "пошта" NewPF1 для користувача Jason.</span><span class="sxs-lookup"><span data-stu-id="def13-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="def13-104">Add-RecipientPermission-Identity ' NewPF1 '-довірена особа "Джейсон"-Accepправами "SendAs"</span><span class="sxs-lookup"><span data-stu-id="def13-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="def13-105">Докладні відомості про синтаксис і параметри наведено в статті [призначення дозволів "Надіслати як" або "Надіслати від імені" для спільних папок із підтримкою пошти](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="def13-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

