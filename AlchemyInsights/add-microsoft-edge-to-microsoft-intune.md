---
title: Додавання Microsoft EDGE до Microsoft InTune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194580"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="d15e6-102">Додавання Microsoft EDGE до Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="d15e6-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="d15e6-103">Щоб мати змогу розгортати, настроювати, відстежувати та захищати Microsoft EDGE для Windows 10, спочатку потрібно додати її до Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="d15e6-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="d15e6-104">Inune підтримує Microsoft EDGE 77 і новіші версії.</span><span class="sxs-lookup"><span data-stu-id="d15e6-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="d15e6-105">Inune виявляє всі попередньо доступні інсталяції Microsoft EDGE.</span><span class="sxs-lookup"><span data-stu-id="d15e6-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="d15e6-106">Якщо Microsoft EDGE інстальовано в контексті користувача, інсталяція системи призведе до перезаписування інсталяції в контексті користувача.</span><span class="sxs-lookup"><span data-stu-id="d15e6-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="d15e6-107">Якщо Microsoft EDGE інстальовано в системному контексті, буде повідомлено про успішність інсталяції.</span><span class="sxs-lookup"><span data-stu-id="d15e6-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="d15e6-108">Попередньо інстальовані Microsoft EDGE 77 і пізніші версії, для всіх каналів у контексті користувача буде замінено Microsoft EDGE, інстальованим в системному контексті.</span><span class="sxs-lookup"><span data-stu-id="d15e6-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="d15e6-109">**Передумовою**</span><span class="sxs-lookup"><span data-stu-id="d15e6-109">**Prerequisite**</span></span>

<span data-ttu-id="d15e6-110">Windows 10 версії 1709 або пізніші версії</span><span class="sxs-lookup"><span data-stu-id="d15e6-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="d15e6-111">**Кроки, щоб додати край до Inune**</span><span class="sxs-lookup"><span data-stu-id="d15e6-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="d15e6-112">[Настройте програму в програмі Inune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d15e6-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="d15e6-113">[Настройте відомості про програму](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d15e6-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="d15e6-114">[Настроювання параметрів програми](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d15e6-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="d15e6-115">[Виберіть теги області (необов'язково)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d15e6-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="d15e6-116">[Додайте програму](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d15e6-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="d15e6-117">Докладні відомості наведено в статті [Виправлення неполадок](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d15e6-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




