---
title: Виправлення неполадок, які заборонено доступ до повідомлень OneDrive, для бізнес-сайтів
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051626"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="7cde9-102">Виправлення неполадок, які заборонено доступ до повідомлень OneDrive, для бізнес-сайтів</span><span class="sxs-lookup"><span data-stu-id="7cde9-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="7cde9-103">Ця проблема найчастіше виникає, коли користувач видаляється і повторно створюється з одного учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="7cde9-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="7cde9-104">Новий обліковий запис створюється за допомогою різних PUID (унікальний ІДЕНТИФІКАТОР паспорта) значення.</span><span class="sxs-lookup"><span data-stu-id="7cde9-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="7cde9-105">Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний PUID.</span><span class="sxs-lookup"><span data-stu-id="7cde9-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="7cde9-106">Другий сценарій передбачає синхронізацію каталогів із організаційною одиницею Active Directory (ОП).</span><span class="sxs-lookup"><span data-stu-id="7cde9-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="7cde9-107">Якщо користувачі вже ввійшли до SharePoint, а потім переміщуються до іншого підрозділу та повторно з SharePoint, вони можуть виникати з цієї проблеми.</span><span class="sxs-lookup"><span data-stu-id="7cde9-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="7cde9-108">Щоб вирішити цю проблему, слід відновити початковий UPN, з кроками у статті, [відновити користувача в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="7cde9-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="7cde9-109">Якщо не вдається відновити вихідний користувач слід видалити старого користувача з OneDrive сайту, за допомогою цих дій, [видалення користувача з відомості про користувача списку]().</span><span class="sxs-lookup"><span data-stu-id="7cde9-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="7cde9-110">Після цього, ви можете перевірити, користувач має права адміністратора на OneDrive сайт, виконавши дії, щоб [Додати адміністратора для користувача onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="7cde9-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="7cde9-111">Докладніші відомості про рівні дозволів наведено в статті, які [розуміють рівні дозволів у програмі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="7cde9-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
