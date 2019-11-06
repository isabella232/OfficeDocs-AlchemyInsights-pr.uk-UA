---
title: 2609-збереження-або-Витребування електронної інформації-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994106"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="c2ddd-102">Не вдалося видалити елементи SharePoint Online або OneDrive, для бізнесу</span><span class="sxs-lookup"><span data-stu-id="c2ddd-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="c2ddd-103">Можливо, вам або вашим користувачам не вдається видалити елементи в SharePoint Online або OneDrive для бізнесу, оскільки політика збереження, підпис збереження або пошук необхідної інформації застосовується до SharePoint OneDrive сайту або певного елемента.</span><span class="sxs-lookup"><span data-stu-id="c2ddd-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="c2ddd-104">Це включає в себе не вдалося видалити документ, версію документа, папку, бібліотеку документів, список, додаток, сайт або колекцію сайтів.</span><span class="sxs-lookup"><span data-stu-id="c2ddd-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="c2ddd-105">Нижче наведено кілька прикладів повідомлень про помилки, які можуть бути отримані під час спроби видалити елемент, який зберігається:</span><span class="sxs-lookup"><span data-stu-id="c2ddd-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="c2ddd-106">"Цей сайт не можна видалити, оскільки він входить до складу" утримання Витребування та збереження "</span><span class="sxs-lookup"><span data-stu-id="c2ddd-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="c2ddd-107">"Цей сайт має політику відповідності встановлено блокувати видалення"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="c2ddd-108">"Політика відповідності в даний час блокує видалення цього сайту"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="c2ddd-109">"Колекцію сайтів не можна видалити, оскільки вона містить сайти, які входять до складу" утримання та збереження Витребування "</span><span class="sxs-lookup"><span data-stu-id="c2ddd-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="c2ddd-110">"Ви повинні видалити всі елементи в цій папці, перш ніж видалити папку"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="c2ddd-111">"Не вдалося видалити версії цього елемента, оскільки він перебуває в політиці утримання або збереження"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="c2ddd-112">"Елемент не можна видалити під час утримання"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="c2ddd-113">"Підпис, застосований до цього елемента, запобігає редагованим або видаленим"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="c2ddd-114">"Не вдається видалити список під час утримання або збереження політики"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="c2ddd-115">"Список не можна видалити, якщо його заблоковано, або якщо до нього застосовано політику збереження"</span><span class="sxs-lookup"><span data-stu-id="c2ddd-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="c2ddd-116">Щоб видалити елементи в одному з цих сценаріїв, політики збереження, Мітки збереження або утримання збереження даних має бути видалено (або сайт має бути виключено з політики зберігання).</span><span class="sxs-lookup"><span data-stu-id="c2ddd-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="c2ddd-117">Потрібно або вимкнути або виключити відповідне утримання, яке спричиняє цю проблему.</span><span class="sxs-lookup"><span data-stu-id="c2ddd-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="c2ddd-118">Після того, як буде видалено політику збереження або утримання, може тривати до 24 годин, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="c2ddd-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="c2ddd-119">Щоб отримати відомості про різні функції збереження та утримання, які можна застосувати до сайтів SharePoint і облікових записів OneDrive, перегляньте одну з наведених нижче розділів.</span><span class="sxs-lookup"><span data-stu-id="c2ddd-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="c2ddd-120">Огляд політик збереження</span><span class="sxs-lookup"><span data-stu-id="c2ddd-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="c2ddd-121">Огляд підписів збереження</span><span class="sxs-lookup"><span data-stu-id="c2ddd-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="c2ddd-122">Керування утриманнями у розширеному Витребування електронної інформації</span><span class="sxs-lookup"><span data-stu-id="c2ddd-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="c2ddd-123">Витребування електронної інформації містить</span><span class="sxs-lookup"><span data-stu-id="c2ddd-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="c2ddd-124">Правила закриття та видалення застарілих сайтів</span><span class="sxs-lookup"><span data-stu-id="c2ddd-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
