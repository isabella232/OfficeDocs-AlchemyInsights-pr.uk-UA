---
title: Надати користувачам доступ до SharePoint і OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736668"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="7b44c-102">Надати користувачам доступ до SharePoint і OneDrive</span><span class="sxs-lookup"><span data-stu-id="7b44c-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="7b44c-103">Ця проблема найчастіше виникає, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="7b44c-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="7b44c-104">Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення.</span><span class="sxs-lookup"><span data-stu-id="7b44c-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="7b44c-105">Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID.</span><span class="sxs-lookup"><span data-stu-id="7b44c-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="7b44c-106">Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП).</span><span class="sxs-lookup"><span data-stu-id="7b44c-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="7b44c-107">Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.</span><span class="sxs-lookup"><span data-stu-id="7b44c-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="7b44c-108">Для вирішення цієї проблеми слід відновити оригінальний УПН з дії, зазначені в статті,[відновити користувача у службі Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="7b44c-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="7b44c-109">Після того, як це буде зроблено, ви можете перевірити, користувач має права адміністратора на сайті OneDrive, виконавши кроки, щоб [Додати адміністратор в для користувача OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="7b44c-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="7b44c-110">Для отримання додаткової інформації на рівні дозволів перегляньте статтю, [розуміння рівнів дозволів в SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="7b44c-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
