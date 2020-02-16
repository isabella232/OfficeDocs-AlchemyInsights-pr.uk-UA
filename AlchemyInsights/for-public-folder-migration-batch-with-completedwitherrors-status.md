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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043629"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Для спільної папки міграції пакета з Повзвєпомилками стан

Виконайте такі дії для завершення пакета, пропускаючи великі/погані елементи: 
1. Затвердити пропущені елементи пакета міграції:

    Набір-Мізаціїпакетна \<назва>-відповідні елементи 
2. Використайте наведену нижче команду, щоб затвердити пропущені елементи на запити міграції, які "синхронізовано", але не завершено:

    $pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-Включаєпорт; Для кожного ($i в $pf) {Якщо ($i. LargeItemsEncountered-gt 0-або $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Ідентифікація. ідентифікатор _ елемента ([Дата й час]:: UtcNow)}}
3. Пакет міграції та запити повинні поновлювати та завершити через кілька хвилин.

