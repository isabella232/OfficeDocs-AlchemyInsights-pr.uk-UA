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
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797569"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="98f27-102">Відновлення видаленого файлу або папки</span><span class="sxs-lookup"><span data-stu-id="98f27-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="98f27-103">SharePoint Online зберігає резервні копії всього вмісту протягом 14 додаткових днів після фактичного видалення.</span><span class="sxs-lookup"><span data-stu-id="98f27-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="98f27-104">Якщо не вдалося відновити вміст за допомогою кошика або відновлення файлів, адміністратор може звернутися до служби підтримки Microsoft, щоб надіслати запит на відновлення в будь-який час у вікні 14 днів.</span><span class="sxs-lookup"><span data-stu-id="98f27-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="98f27-105">Відновлення з резервних копій можна виконати лише для колекцій сайтів або підсайтів, а не для окремих файлів, списків або бібліотек.</span><span class="sxs-lookup"><span data-stu-id="98f27-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="98f27-106">Під час видалення елемента або сайту зі служби SharePoint його не можна видалити відразу.</span><span class="sxs-lookup"><span data-stu-id="98f27-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="98f27-107">Видалені елементи потрапляють до кошика, де зберігаються деякий час.</span><span class="sxs-lookup"><span data-stu-id="98f27-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="98f27-108">Протягом цього періоду можна відновити видалені елементи до вихідного розташування.</span><span class="sxs-lookup"><span data-stu-id="98f27-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="98f27-109">Щоб дізнатися більше, перейдіть за посиланнями нижче.</span><span class="sxs-lookup"><span data-stu-id="98f27-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="98f27-110">[Відновлення об'єктів у кошику на сайті SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="98f27-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="98f27-111">Відновлення видалених файлів або папок у OneDrive</span><span class="sxs-lookup"><span data-stu-id="98f27-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="98f27-112">Відновлення видаленої колекції сайтів (включно з групами, зв'язками та іншими сайтами)</span><span class="sxs-lookup"><span data-stu-id="98f27-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="98f27-113">Відновлення видаленого сайту OneDrive</span><span class="sxs-lookup"><span data-stu-id="98f27-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="98f27-114">Для дій групового кошика адміністратори можуть враховувати використання служби [SharePoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="98f27-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="98f27-115">**Функція відновлення файлів**</span><span class="sxs-lookup"><span data-stu-id="98f27-115">**Files Restore feature**</span></span>

<span data-ttu-id="98f27-116">Якщо у вас багато файлів OneDrive або файли SharePoint видаляються, перезаписані, пошкоджені або заражені зловмисними програмами, ви можете відновити всі файли OneDrive або бібліотеку SharePoint до попереднього часу за допомогою функції відновлення файлів.</span><span class="sxs-lookup"><span data-stu-id="98f27-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="98f27-117">Відновлення бібліотеки OneDrive</span><span class="sxs-lookup"><span data-stu-id="98f27-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="98f27-118">Відновлення бібліотеки документів</span><span class="sxs-lookup"><span data-stu-id="98f27-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

