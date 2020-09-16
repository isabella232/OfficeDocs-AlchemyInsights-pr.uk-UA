---
title: Для пакета перенесення спільних папок із статусом CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744134"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="654ad-102">Для пакета перенесення спільних папок із статусом CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="654ad-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="654ad-103">Виконайте наведені нижче дії, щоб завершити пакет, пропускаючи великі або погані елементи.</span><span class="sxs-lookup"><span data-stu-id="654ad-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="654ad-104">Затвердити пропущені пункти для пакета перенесення:</span><span class="sxs-lookup"><span data-stu-id="654ad-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="654ad-105">Виконайте таку команду, щоб затвердити пропущені елементи для запитів міграції, які "синхронізовано", але не завершено:</span><span class="sxs-lookup"><span data-stu-id="654ad-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="654ad-106">Пакет перенесення та запити слід відновити та завершити протягом кількох хвилин.</span><span class="sxs-lookup"><span data-stu-id="654ad-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

