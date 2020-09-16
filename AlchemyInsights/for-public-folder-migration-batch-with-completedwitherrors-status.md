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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Для пакета перенесення спільних папок із статусом CompletedWithErrors

Виконайте наведені нижче дії, щоб завершити пакет, пропускаючи великі або погані елементи. 
1. Затвердити пропущені пункти для пакета перенесення:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Виконайте таку команду, щоб затвердити пропущені елементи для запитів міграції, які "синхронізовано", але не завершено:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Пакет перенесення та запити слід відновити та завершити протягом кількох хвилин.

