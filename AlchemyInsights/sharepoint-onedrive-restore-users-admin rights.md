---
title: Усунення несправностей доступ заборонено повідомлень до OneDrive для бізнес сайтів
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232568"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="88f85-102">Усунення несправностей доступ заборонено повідомлень до OneDrive для бізнес сайтів</span><span class="sxs-lookup"><span data-stu-id="88f85-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="88f85-103">Ця проблема найчастіше виникає, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="88f85-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="88f85-104">Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення.</span><span class="sxs-lookup"><span data-stu-id="88f85-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="88f85-105">Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID.</span><span class="sxs-lookup"><span data-stu-id="88f85-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="88f85-106">Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП).</span><span class="sxs-lookup"><span data-stu-id="88f85-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="88f85-107">Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.</span><span class="sxs-lookup"><span data-stu-id="88f85-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="88f85-108">Для вирішення цієї проблеми слід відновити оригінальний УПН з дії, зазначені в статті,[відновити користувача у службі Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="88f85-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="88f85-109">Якщо не вдалося відновити оригінальний користувача слід видалити старі користувача з сайту OneDrive, за допомогою цих кроків, [Видалити користувача зі списку відомостей про користувача]().</span><span class="sxs-lookup"><span data-stu-id="88f85-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="88f85-110">Після того, як це буде зроблено, ви можете перевірити, користувач має права адміністратора на сайті OneDrive, виконавши кроки, щоб [Додати адміністратор в для користувача OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="88f85-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="88f85-111">Для отримання додаткової інформації на рівні дозволів перегляньте статтю, [розуміння рівнів дозволів в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="88f85-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
