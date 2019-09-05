---
title: Усунення несправностей у доступі повідомлення
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751297"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="c5ba1-102">Виправлення неполадок із Забороними доступом у центрі адміністрування SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="c5ba1-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="c5ba1-103">Якщо ви отримуєте повідомлення про відмову в доступі під час спроби перейти до центру адміністрування SharePoint/OneDrive, будь ласка, переконайтеся, що ви [призначаєте ліцензію користувачу](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="c5ba1-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="c5ba1-104">Якщо користувач має ліцензію, ви також повинні переконатися, що вони [призначені роль адміністратора](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , які можуть отримати доступ до центрів адміністрування.</span><span class="sxs-lookup"><span data-stu-id="c5ba1-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="c5ba1-105">Ця проблема також може виникати, коли користувач видаляється і повторно створюється з одного учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="c5ba1-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c5ba1-106">Новий обліковий запис створюється за допомогою різних PUID (унікальний ІДЕНТИФІКАТОР паспорта) значення.</span><span class="sxs-lookup"><span data-stu-id="c5ba1-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c5ba1-107">Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний PUID.</span><span class="sxs-lookup"><span data-stu-id="c5ba1-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c5ba1-108">Другий сценарій передбачає синхронізацію каталогів із організаційною одиницею Active Directory (ОП).</span><span class="sxs-lookup"><span data-stu-id="c5ba1-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c5ba1-109">Якщо користувачі вже ввійшли до SharePoint, а потім переміщуються до іншого підрозділу та повторно з SharePoint, вони можуть виникати з цієї проблеми.</span><span class="sxs-lookup"><span data-stu-id="c5ba1-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c5ba1-110">Щоб вирішити цю проблему, слід відновити початковий UPN, з кроками у статті, [відновити користувача в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c5ba1-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="c5ba1-111">Примітка: Якщо Центр адміністрування OneDrive або SharePoint недоступний для кількох користувачів, які раніше мали доступ, може виникнути проблема з тимчасовим обслуговуванням.</span><span class="sxs-lookup"><span data-stu-id="c5ba1-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="c5ba1-112">[Перегляньте приладну дошку справності служб](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c5ba1-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


