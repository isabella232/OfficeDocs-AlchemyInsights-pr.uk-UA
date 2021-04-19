---
title: Пристрої Configuration Manager, яких немає на порталі
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817265"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="c7036-102">Пристрої Configuration Manager, яких немає на порталі</span><span class="sxs-lookup"><span data-stu-id="c7036-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="c7036-103">Щоб синхронізувати пристрій, для локального сервера, на якому розміщено роль точки підключення до служби, мають бути доступні [обов’язкові кінцеві точки Інтернету](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints).</span><span class="sxs-lookup"><span data-stu-id="c7036-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="c7036-104">Щоб вирішити проблеми із синхронізацією пристрою, ознайомтеся з журналом **CMGatewaySyncUploadWorker.log**, що розташований у точці підключення до служби.</span><span class="sxs-lookup"><span data-stu-id="c7036-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="c7036-105">Докладні відомості про [Вкладення клієнта в Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="c7036-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
