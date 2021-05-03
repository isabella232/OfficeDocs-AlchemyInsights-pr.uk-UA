---
title: Вирішення проблем із завданням служби імпорту
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125777"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="1712a-102">Вирішення проблем із завданням служби імпорту</span><span class="sxs-lookup"><span data-stu-id="1712a-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="1712a-103">Якщо виникають проблеми з завданнями імпорту служб, які застрягли або виникли помилки, перевірте та спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="1712a-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="1712a-104">Перегляньте розмір файлу PST.</span><span class="sxs-lookup"><span data-stu-id="1712a-104">Review the size of of the PST file.</span></span> <span data-ttu-id="1712a-105">Максимальний рекомендований розмір файлу PST для імпорту – 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="1712a-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="1712a-106">Якщо ви підозрюєте, що елементи через пошкодження пропущено, Scanpst.exe діагностувати та виправити помилки у файлах PST.</span><span class="sxs-lookup"><span data-stu-id="1712a-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="1712a-107">Якщо під час імпорту відображається помилка "MapiExceptionShutoffQuotaExceeded", переконайтеся, що цільовій поштовій скриньці достатньо потужності для імпорту потрібних PST-файлів.</span><span class="sxs-lookup"><span data-stu-id="1712a-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="1712a-108">Докладні відомості про виправлення неполадок із завданням імпорту PST-файлів див. в цьому [низці.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="1712a-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="1712a-109">Відомості про те, як вирішувати проблеми під час імпорту файлів PST Outlook див. в статті Вирішення проблем з імпортом файлу OUTLOOK [(microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="1712a-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>