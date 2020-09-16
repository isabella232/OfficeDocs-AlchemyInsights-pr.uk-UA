---
title: Проблеми з продуктивністю – SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771265"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="48f23-102">Служба SharePoint або OneDrive низька, недоступна або недоступна для кількох користувачів</span><span class="sxs-lookup"><span data-stu-id="48f23-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="48f23-103">Якщо ви не маєте доступу до кількох користувачів, які раніше мали доступ до служби "OneDrive" або сайту SharePoint, може виникнути тимчасова проблема з обслуговуванням.</span><span class="sxs-lookup"><span data-stu-id="48f23-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="48f23-104">[Перевірте приладну дошку справності служби](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="48f23-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="48f23-105">**Додавання та Ліцензія користувача**</span><span class="sxs-lookup"><span data-stu-id="48f23-105">**Add and license the user**</span></span>

<span data-ttu-id="48f23-106">Переконайтеся, що ви [призначите ліцензії користувачам у програмі Microsoft 365 для бізнесу](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="48f23-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="48f23-107">**Призначення дозволів**</span><span class="sxs-lookup"><span data-stu-id="48f23-107">**Assign Permissions**</span></span>

<span data-ttu-id="48f23-108">Якщо користувач надав ліцензію SharePoint і продовжує отримувати повідомлення про відмову в доступі, переконайтеся, що вони мають [відповідний рівень дозволів](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="48f23-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="48f23-109">**Використання функції "запит на доступ"**</span><span class="sxs-lookup"><span data-stu-id="48f23-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="48f23-110">[Функція "запит на доступ](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) " дає змогу користувачам запитувати доступ до вмісту, у якому вони зараз не мають дозволу на перегляд.</span><span class="sxs-lookup"><span data-stu-id="48f23-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="48f23-111">**Дозволити настроюваний сценарій може спричинити проблеми з заперечуванням Access**</span><span class="sxs-lookup"><span data-stu-id="48f23-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="48f23-112">Існують певні сценарії, у яких функція " *дозволити настроюваний скрипт* " може представляти відмовлено в доступі.</span><span class="sxs-lookup"><span data-stu-id="48f23-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="48f23-113">Список функцій, які постраждали, міркувань безпеки та можливість вимкнення функції.</span><span class="sxs-lookup"><span data-stu-id="48f23-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="48f23-114">Перейдіть на веб [-сайті дозволити або заборонити настроюваний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="48f23-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

