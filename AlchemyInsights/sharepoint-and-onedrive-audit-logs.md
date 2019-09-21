---
title: Класичні звіти журналу аудиту SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068044"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="5b92d-102">Журнали аудиту SharePoint і OneDrive</span><span class="sxs-lookup"><span data-stu-id="5b92d-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="5b92d-103">**Служби SharePoint і OneDrive сучасних Unified аудиту журнали відповідності**</span><span class="sxs-lookup"><span data-stu-id="5b92d-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="5b92d-104">Увімкнення/вимкнення єдиного аудиту журналювання</span><span class="sxs-lookup"><span data-stu-id="5b92d-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="5b92d-105">У SharePoint або OneDrive не потрібна додаткова конфігурація.</span><span class="sxs-lookup"><span data-stu-id="5b92d-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="5b92d-106">Використання аудиту журналювання пошук для перевірки діяльності файлів (ів), папок (ів), користувачів (ів), дозволи:</span><span class="sxs-lookup"><span data-stu-id="5b92d-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="5b92d-107">Файл і сторінка діяльність</span><span class="sxs-lookup"><span data-stu-id="5b92d-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="5b92d-108">Папки діяльності</span><span class="sxs-lookup"><span data-stu-id="5b92d-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="5b92d-109">Дії з надсилання й отримання доступу</span><span class="sxs-lookup"><span data-stu-id="5b92d-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="5b92d-110">Дії синхронізації</span><span class="sxs-lookup"><span data-stu-id="5b92d-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="5b92d-111">Діяльність адміністрування сайту</span><span class="sxs-lookup"><span data-stu-id="5b92d-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="5b92d-112">Щоб отримати додаткові відомості про отримання цих подій, перегляньте статтю [Пошук журналу аудиту](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="5b92d-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="5b92d-113">**Журнали для класичного аудиту SharePoint**</span><span class="sxs-lookup"><span data-stu-id="5b92d-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="5b92d-114">Ми перенесено спо-Legacy аудиту в уніфікований аудит журналу (АЛЬ).</span><span class="sxs-lookup"><span data-stu-id="5b92d-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="5b92d-115">Це, по суті, означає, що всі звіти по аудиті аудиту тепер будуть проходити через АЛЬ, а застарілі аудиторські сигнали були перенесені в АЛЬ.</span><span class="sxs-lookup"><span data-stu-id="5b92d-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="5b92d-116">Ключові зміни:</span><span class="sxs-lookup"><span data-stu-id="5b92d-116">Key changes:</span></span>

- <span data-ttu-id="5b92d-117">Обрізка як можливість недоступна.</span><span class="sxs-lookup"><span data-stu-id="5b92d-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="5b92d-118">Розділ, на якому ви вибираєте конкретні події для аудиту, недоступний.</span><span class="sxs-lookup"><span data-stu-id="5b92d-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="5b92d-119">Перегляньте [цей документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) , щоб отримати повний список відстежуваної події за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="5b92d-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="5b92d-120">Параметр "розташування" під **настроюванними звітами** недоступний.</span><span class="sxs-lookup"><span data-stu-id="5b92d-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="5b92d-121">"Відкриття або завантаження документів" події недоступні.</span><span class="sxs-lookup"><span data-stu-id="5b92d-121">“Opening or downloading documents” events is NOT available.</span></span> 

