---
title: Виправлення неполадок із відхилень у програмі Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707975"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="37de9-102">Виправлення неполадок із Заперечуванням повідомлень у центрі адміністрування SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="37de9-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="37de9-103">Якщо ви отримуєте повідомлення про відмову в доступі під час спроби перейти до центру адміністрування SharePoint або OneDrive, переконайтеся, що ви [призначите ліцензію користувачу](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="37de9-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="37de9-104">Якщо користувач має ліцензію, слід також переконатися, що їм [призначено роль адміністратора](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , які можуть отримати доступ до центрів адміністрування.</span><span class="sxs-lookup"><span data-stu-id="37de9-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="37de9-105">Ця проблема також може виникати, коли користувач видаляється та повторно створюється за допомогою одного імені учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="37de9-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="37de9-106">Новий обліковий запис створюється за допомогою іншого значення "PUID" (унікальний ІДЕНТИФІКАТОР паспорта).</span><span class="sxs-lookup"><span data-stu-id="37de9-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="37de9-107">Коли користувач спробує отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний ідентифікатор.</span><span class="sxs-lookup"><span data-stu-id="37de9-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="37de9-108">Другий сценарій передбачає синхронізацію служби каталогів за допомогою організаційної одиниці Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="37de9-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="37de9-109">Якщо користувачі вже ввійшли у службу SharePoint, а потім переміщуються до іншої програми SharePoint, вони можуть виникнути під час цієї проблеми.</span><span class="sxs-lookup"><span data-stu-id="37de9-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="37de9-110">Щоб вирішити цю проблему, потрібно відновити початковий УПН, виконавши кроки, описані в статті, [відновлення користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="37de9-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="37de9-111">Примітка. Якщо Центр адміністрування Onedriveабо SharePoint недоступний для кількох користувачів, які раніше мали доступ, може виникнути тимчасова проблема служби.</span><span class="sxs-lookup"><span data-stu-id="37de9-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="37de9-112">[Перевірте приладну дошку справності служби](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="37de9-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


