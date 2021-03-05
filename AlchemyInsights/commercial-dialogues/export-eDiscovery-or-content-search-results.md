---
title: Експорт електронної інформації та результати пошуку вмісту
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483733"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="6b34a-102">Експорт електронної інформації та результати пошуку вмісту</span><span class="sxs-lookup"><span data-stu-id="6b34a-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="6b34a-103">Можливо, знадобиться експортувати результати пошуку до PST-файлу (з електронної пошти) або до рідних документів Office (зі служби SharePoint і OneDrive для бізнесу).</span><span class="sxs-lookup"><span data-stu-id="6b34a-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="6b34a-104">Якщо так, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="6b34a-104">If so, do the following:</span></span>

- <span data-ttu-id="6b34a-105">Переконайтеся, що ваш обліковий запис призначено відповідних дозволів для експорту.</span><span class="sxs-lookup"><span data-stu-id="6b34a-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="6b34a-106">Докладні відомості наведено в статті [призначення дозволів на відкриття електронної](https://go.microsoft.com/fwlink/?linkid=2102406)інформації.</span><span class="sxs-lookup"><span data-stu-id="6b34a-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="6b34a-107">Переконайтеся, що ваш комп'ютер виконав всі [попередні вимоги](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="6b34a-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="6b34a-108">Підтримуються не всі браузери, як-от Chrome.</span><span class="sxs-lookup"><span data-stu-id="6b34a-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="6b34a-109">Щоб експортувати дані з пошуку вмісту, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="6b34a-109">To export from a Content Search: a.</span></span> <span data-ttu-id="6b34a-110">Перейдіть до [центру відповідності & безпеки](https://protection.office.com/contentsearch) та натисніть кнопку **Пошук**, а потім виберіть пункт **Пошук вмісту**.</span><span class="sxs-lookup"><span data-stu-id="6b34a-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="6b34a-111">На сторінці **Пошук вмісту** виберіть збережений пошуковий запит.</span><span class="sxs-lookup"><span data-stu-id="6b34a-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="6b34a-112">b.</span><span class="sxs-lookup"><span data-stu-id="6b34a-112">b.</span></span> <span data-ttu-id="6b34a-113">В області відомостей у розділі **Експорт результатів до комп'ютера** натисніть кнопку **почати експорт**.</span><span class="sxs-lookup"><span data-stu-id="6b34a-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="6b34a-114">Якщо ви експортуєте понад 100K поштові скриньки, вам знадобиться використовувати PowerShell для завантаження результатів експорту.</span><span class="sxs-lookup"><span data-stu-id="6b34a-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="6b34a-115">Докладні відомості наведено в статті [Експорт результатів із понад 100K поштових скриньок](https://go.microsoft.com/fwlink/?linkid=2143861).</span><span class="sxs-lookup"><span data-stu-id="6b34a-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="6b34a-116">Докладні відомості наведено в статті [Експорт результатів пошуку вмісту](https://go.microsoft.com/fwlink/?linkid=2102118).</span><span class="sxs-lookup"><span data-stu-id="6b34a-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>