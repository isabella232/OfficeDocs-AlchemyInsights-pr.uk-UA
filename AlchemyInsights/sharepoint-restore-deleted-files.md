---
title: Відновити видалений файл або папку
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 1672f425719597b93b8ef05865797714c3b19e42
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758926"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="af2c1-102">Відновити видалений файл або папку</span><span class="sxs-lookup"><span data-stu-id="af2c1-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="af2c1-103">SharePoint Online зберігає резервні копії всіх контенту на 14 додаткових днів за межами фактичної видалення.</span><span class="sxs-lookup"><span data-stu-id="af2c1-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="af2c1-104">Якщо вміст не можна відновити за допомогою кошика або відновити файли, адміністратор зверніться до служби підтримки Microsoft просити відновити будь-який час всередині вікна 14 день.</span><span class="sxs-lookup"><span data-stu-id="af2c1-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="af2c1-105">Реставрацій резервні копії може бути завершено лише для колекцій сайтів або дочірніх сайтів, не для певних файлів, списків і бібліотек.</span><span class="sxs-lookup"><span data-stu-id="af2c1-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="af2c1-106">При видаленні елемента або сайт з Sharepoint, він негайно не видаляється.</span><span class="sxs-lookup"><span data-stu-id="af2c1-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="af2c1-107">Видалені елементи потрапляють до кошика для певного періоду часу.</span><span class="sxs-lookup"><span data-stu-id="af2c1-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="af2c1-108">За цей час можна буде відновити елементи, які ви видалили на колишнє місце.</span><span class="sxs-lookup"><span data-stu-id="af2c1-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="af2c1-109">Для отримання додаткової інформації будь ласка, відвідайте нижче посиланнями.</span><span class="sxs-lookup"><span data-stu-id="af2c1-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="af2c1-110">[Відновити елементи з кошика сайту SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="af2c1-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="af2c1-111">Відновити видалені файли або папки в OneDrive</span><span class="sxs-lookup"><span data-stu-id="af2c1-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="af2c1-112">Відновлення видаленої вузлів (у тому числі групи, зв'язку та інших сайтів)</span><span class="sxs-lookup"><span data-stu-id="af2c1-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="af2c1-113">Відновлення видаленої сайт OneDrive</span><span class="sxs-lookup"><span data-stu-id="af2c1-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="af2c1-114">Для оптових recycle bin дії адміністратори можуть розглянути можливість використання [Sharepoint онлайн PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="af2c1-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="af2c1-115">**Функція відновлення файлів**</span><span class="sxs-lookup"><span data-stu-id="af2c1-115">**Files Restore feature**</span></span>

<span data-ttu-id="af2c1-116">Якщо багато OneDrive або SharePoint файлів отримати видалені, перезаписані, пошкоджена або заражені шкідливим, ви можете відновити всю медіатеку OneDrive або SharePoint попередній час за допомогою функцією відновлення файлів.</span><span class="sxs-lookup"><span data-stu-id="af2c1-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="af2c1-117">Відновити OneDrive бібліотека</span><span class="sxs-lookup"><span data-stu-id="af2c1-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="af2c1-118">Відновити бібліотеки документів</span><span class="sxs-lookup"><span data-stu-id="af2c1-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

