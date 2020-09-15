---
title: Виправлення неполадок із відхилень у програмі Access для веб-сайтів у службі OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670637"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="31c93-102">Виправлення неполадок із відхилень у програмі Access для веб-сайтів у службі OneDrive</span><span class="sxs-lookup"><span data-stu-id="31c93-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="31c93-103">Ця проблема найчастіше виникає, коли користувач видаляється та повторно створюється за допомогою одного імені учасника-користувача (UPN).</span><span class="sxs-lookup"><span data-stu-id="31c93-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="31c93-104">Новий обліковий запис створюється за допомогою іншого значення "PUID" (унікальний ІДЕНТИФІКАТОР паспорта).</span><span class="sxs-lookup"><span data-stu-id="31c93-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="31c93-105">Коли користувач спробує отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний ідентифікатор.</span><span class="sxs-lookup"><span data-stu-id="31c93-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="31c93-106">Другий сценарій передбачає синхронізацію служби каталогів за допомогою організаційної одиниці Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="31c93-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="31c93-107">Якщо користувачі вже ввійшли у службу SharePoint, а потім переміщуються до іншої програми SharePoint, вони можуть виникнути під час цієї проблеми.</span><span class="sxs-lookup"><span data-stu-id="31c93-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="31c93-108">Щоб вирішити цю проблему, потрібно відновити початковий UPN, виконавши кроки, описані в статті, [відновлення користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="31c93-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="31c93-109">Якщо ви не можете відновити початковий користувач, який ви маєте видалити старий користувач із сайту OneDrive, виконавши наведені нижче дії, [видаліть користувача зі списку відомостей про користувача]().</span><span class="sxs-lookup"><span data-stu-id="31c93-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="31c93-110">Після цього ви можете перевірити, чи користувач має права адміністратора на веб-сайт OneDrive, виконавши вказівки з [Додавання адміністратора для onedrive користувача](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="31c93-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="31c93-111">Докладні відомості про рівні дозволів наведено в статті, [розумінні рівнів дозволів у службі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="31c93-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
