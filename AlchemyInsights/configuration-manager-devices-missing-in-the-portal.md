---
title: Пристрої Configuration Manager, яких немає на порталі
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790238"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="9aae9-102">Пристрої Configuration Manager, яких немає на порталі</span><span class="sxs-lookup"><span data-stu-id="9aae9-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="9aae9-103">Щоб синхронізувати пристрій, для локального сервера, на якому розміщено роль точки підключення до служби, мають бути доступні [обов’язкові кінцеві точки Інтернету](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints).</span><span class="sxs-lookup"><span data-stu-id="9aae9-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="9aae9-104">Щоб вирішити проблеми із синхронізацією пристрою, ознайомтеся з журналом **CMGatewaySyncUploadWorker.log**, що розташований у точці підключення до служби.</span><span class="sxs-lookup"><span data-stu-id="9aae9-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="9aae9-105">Докладні відомості про [Вкладення клієнта в Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="9aae9-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
