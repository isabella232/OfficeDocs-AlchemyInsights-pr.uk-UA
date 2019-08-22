---
title: 'Усунення проблем: відмовлено у доступі до повідомлення'
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503566"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="07de8-102">Усунення проблем: відмовлено у доступі до повідомлення центру адміністрування Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="07de8-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="07de8-103">Якщо ви отримуєте в доступі повідомлення при спробі перейдіть до центру адміністрування Sharepoint/OneDrive, будь ласка переконайтесь, що ви [призначите ліцензію для користувача](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="07de8-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="07de8-104">Якщо користувач має ліцензію, ви повинні також переконайтеся, що вони [призначені роль адміністратора](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) доступ адміністратора центрів.</span><span class="sxs-lookup"><span data-stu-id="07de8-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="07de8-105">Ця проблема також може виникнути, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="07de8-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="07de8-106">Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення.</span><span class="sxs-lookup"><span data-stu-id="07de8-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="07de8-107">Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID.</span><span class="sxs-lookup"><span data-stu-id="07de8-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="07de8-108">Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП).</span><span class="sxs-lookup"><span data-stu-id="07de8-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="07de8-109">Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.</span><span class="sxs-lookup"><span data-stu-id="07de8-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="07de8-110">Щоб вирішити цю проблему, слід відновити оригінальний УПН з дії, зазначені в статті, [відновити користувача у службі Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="07de8-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="07de8-111">Примітка: Якщо OneDrive або адміністратор SharePoint центр недоступна для декількох користувачів, які раніше мали доступ, це може бути тимчасова служби питання.</span><span class="sxs-lookup"><span data-stu-id="07de8-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="07de8-112">[Перевірте службу здоров'я приладної дошки](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="07de8-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


