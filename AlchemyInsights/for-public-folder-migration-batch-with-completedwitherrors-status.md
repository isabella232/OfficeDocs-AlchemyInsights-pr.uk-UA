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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Для спільної папки міграції пакета з Повзвєпомилками стан

Виконайте такі дії для завершення пакета, пропускаючи великі/погані елементи: 
1. Затвердити пропущені елементи пакета міграції:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Використайте наведену нижче команду, щоб затвердити пропущені елементи на запити міграції, які "синхронізовано", але не завершено:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Пакет міграції та запити повинні поновлювати та завершити через кілька хвилин.

