---
title: Виправлення неполадок із продуктивністю у OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757906"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="8aa86-102">Виправлення неполадок із продуктивністю у OneDrive</span><span class="sxs-lookup"><span data-stu-id="8aa86-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="8aa86-103">Якщо у вас виникли повільніше, ніж очікувалося, або аналогічні проблеми з продуктивністю у OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8aa86-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="8aa86-104">Переконайтеся, що на [приладній дошці справності](https://portal.office.com/adminportal/home?ref=/servicehealth)немає відомих проблем.</span><span class="sxs-lookup"><span data-stu-id="8aa86-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="8aa86-105">[Активуйте файли на вимогу](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , щоб мати доступ до всіх файлів у службі OneDrive без завантаження всіх їх і використання дискового простору на своєму пристрої.</span><span class="sxs-lookup"><span data-stu-id="8aa86-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="8aa86-106">[Перегляньте практичні поради](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) з планування та продуктивності мережі.</span><span class="sxs-lookup"><span data-stu-id="8aa86-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="8aa86-107">[Максимальна швидкість передавання та завантаження](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), особливо якщо ви синхронізуєте пристрій уперше.</span><span class="sxs-lookup"><span data-stu-id="8aa86-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="8aa86-108">Якщо ви синхронізуєте бібліотеку з більш ніж 100 000, синхронізація OneDrive може здатися надовго, або стан відображає обробку 0KB від xMB. "</span><span class="sxs-lookup"><span data-stu-id="8aa86-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="8aa86-109">Докладні [відомості про синхронізацію понад 100 000 файлів](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , а також [підтримується обмеження onedriy's 300 000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="8aa86-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="8aa86-110">Якщо користувач перевищує обмеження використання, служба SharePoint Online Дроселі будь-які подальші запити з цього облікового запису користувача на короткий період.</span><span class="sxs-lookup"><span data-stu-id="8aa86-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="8aa86-111">Усі дії користувача буде обмежено, коли Дросельний ефект діє.</span><span class="sxs-lookup"><span data-stu-id="8aa86-111">All user actions are throttled while the throttle is in effect.</span></span>
