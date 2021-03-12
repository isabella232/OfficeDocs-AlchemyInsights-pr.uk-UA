---
title: Відновлення видаленого файлу або папки
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707543"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="4ecdf-102">Відновлення видаленого файлу або папки</span><span class="sxs-lookup"><span data-stu-id="4ecdf-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="4ecdf-103">SharePoint Online зберігає резервні копії всього вмісту протягом 14 додаткових днів після фактичного видалення.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="4ecdf-104">Якщо не вдалося відновити вміст за допомогою кошика або відновлення файлів, адміністратор може звернутися до служби підтримки Microsoft, щоб надіслати запит на відновлення в будь-який час у вікні 14 днів.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="4ecdf-105">Відновлення з резервних копій можна виконати лише для колекцій сайтів або підсайтів, а не для окремих файлів, списків або бібліотек.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="4ecdf-106">Під час видалення елемента або сайту зі служби SharePoint його не можна видалити відразу.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="4ecdf-107">Видалені елементи потрапляють до кошика, де зберігаються деякий час.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="4ecdf-108">Протягом цього періоду можна відновити видалені елементи до вихідного розташування.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="4ecdf-109">Щоб дізнатися більше, перейдіть за посиланнями нижче.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="4ecdf-110">[Відновлення об'єктів у кошику на сайті SharePoint](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span><span class="sxs-lookup"><span data-stu-id="4ecdf-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="4ecdf-111">Відновлення видалених файлів або папок у OneDrive</span><span class="sxs-lookup"><span data-stu-id="4ecdf-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="4ecdf-112">Відновлення видаленої колекції сайтів (включно з групами, зв'язками та іншими сайтами)</span><span class="sxs-lookup"><span data-stu-id="4ecdf-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="4ecdf-113">Відновлення видаленого сайту OneDrive</span><span class="sxs-lookup"><span data-stu-id="4ecdf-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="4ecdf-114">Для дій групового кошика адміністратори можуть враховувати використання служби [SharePoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="4ecdf-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="4ecdf-115">**Функція відновлення файлів**</span><span class="sxs-lookup"><span data-stu-id="4ecdf-115">**Files Restore feature**</span></span>

<span data-ttu-id="4ecdf-116">Якщо у вас багато файлів OneDrive або файли SharePoint видаляються, перезаписані, пошкоджені або заражені зловмисними програмами, ви можете відновити всі файли OneDrive або бібліотеку SharePoint до попереднього часу за допомогою функції відновлення файлів.</span><span class="sxs-lookup"><span data-stu-id="4ecdf-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="4ecdf-117">Відновлення бібліотеки OneDrive</span><span class="sxs-lookup"><span data-stu-id="4ecdf-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="4ecdf-118">Відновлення бібліотеки документів</span><span class="sxs-lookup"><span data-stu-id="4ecdf-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

