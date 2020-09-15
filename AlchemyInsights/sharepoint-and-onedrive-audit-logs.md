---
title: Класичні звіти журналу аудиту SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662229"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="d4df6-102">Журнали аудиту SharePoint і OneDrive</span><span class="sxs-lookup"><span data-stu-id="d4df6-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="d4df6-103">Журнали аудиту SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="d4df6-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="d4df6-104">Відстеження успадкованого аудиту в службі єдиного журналу аудиту (UAL).</span><span class="sxs-lookup"><span data-stu-id="d4df6-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="d4df6-105">У всіх звітах про успадковані аудиторські звіти тепер буде здійснюватися через Al, а успадковані сигналах, які було перенесено до UAL.</span><span class="sxs-lookup"><span data-stu-id="d4df6-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="d4df6-106">Основні зміни:</span><span class="sxs-lookup"><span data-stu-id="d4df6-106">Key changes:</span></span>

* <span data-ttu-id="d4df6-107">Функція обрізки недоступна як можливість.</span><span class="sxs-lookup"><span data-stu-id="d4df6-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="d4df6-108">Вибір певних подій для аудиту недоступний.</span><span class="sxs-lookup"><span data-stu-id="d4df6-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="d4df6-109">Зверніться до [цього документа](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) , щоб переглянути повний список перевірених подій, доступних за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="d4df6-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="d4df6-110">Параметр " **розташування** " в розділі " **Настроювані звіти** " недоступний.</span><span class="sxs-lookup"><span data-stu-id="d4df6-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="d4df6-111">Параметр " **відкриття або завантаження** подій для документів" недоступний.</span><span class="sxs-lookup"><span data-stu-id="d4df6-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="d4df6-112">Настроювання параметрів аудиту для колекції сайтів</span><span class="sxs-lookup"><span data-stu-id="d4df6-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="d4df6-113">Служби SharePoint і OneDrive для сучасних уніфікованих журналів аудиту відповідно</span><span class="sxs-lookup"><span data-stu-id="d4df6-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="d4df6-114">Увімкнення та вимкнення журналювання єдиного аудиту</span><span class="sxs-lookup"><span data-stu-id="d4df6-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="d4df6-115">У службі SharePoint або OneDrive не потрібне додаткове настроювання.</span><span class="sxs-lookup"><span data-stu-id="d4df6-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="d4df6-116">Використання функції журналювання аудиту для перевірки діяльності файлів (-ів), папок, користувачів, дозволів:</span><span class="sxs-lookup"><span data-stu-id="d4df6-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="d4df6-117">Дії з файлами та сторінками</span><span class="sxs-lookup"><span data-stu-id="d4df6-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="d4df6-118">Дії з папками</span><span class="sxs-lookup"><span data-stu-id="d4df6-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="d4df6-119">Надання спільного доступу до дій і запитів на доступ</span><span class="sxs-lookup"><span data-stu-id="d4df6-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="d4df6-120">Дії з синхронізації</span><span class="sxs-lookup"><span data-stu-id="d4df6-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="d4df6-121">Дії з адміністрування сайту</span><span class="sxs-lookup"><span data-stu-id="d4df6-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="d4df6-122">Додаткові відомості про те, як отримати ці події, наведено [в статті пошук у журналі аудиту](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d4df6-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
