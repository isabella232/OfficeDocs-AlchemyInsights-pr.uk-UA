---
title: Для спільної папки міграції пакета з Повзвєпомилками стан
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158647"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="283f4-102">Для спільної папки міграції пакета з Повзвєпомилками стан</span><span class="sxs-lookup"><span data-stu-id="283f4-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="283f4-103">Виконайте такі дії для завершення пакета, пропускаючи великі/погані елементи:</span><span class="sxs-lookup"><span data-stu-id="283f4-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="283f4-104">Затвердити пропущені елементи пакета міграції:</span><span class="sxs-lookup"><span data-stu-id="283f4-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="283f4-105">Використайте наведену нижче команду, щоб затвердити пропущені елементи на запити міграції, які "синхронізовано", але не завершено:</span><span class="sxs-lookup"><span data-stu-id="283f4-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="283f4-106">Пакет міграції та запити повинні поновлювати та завершити через кілька хвилин.</span><span class="sxs-lookup"><span data-stu-id="283f4-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

