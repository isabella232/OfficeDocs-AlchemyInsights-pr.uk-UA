---
title: Виправлення неполадок, які заборонено доступ до повідомлень OneDrive, для бізнес-сайтів
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766732"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Виправлення неполадок, які заборонено доступ до повідомлень OneDrive, для бізнес-сайтів

Ця проблема найчастіше виникає, коли користувач видаляється і повторно створюється з одного учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (унікальний ІДЕНТИФІКАТОР паспорта) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний PUID. Другий сценарій передбачає синхронізацію каталогів із організаційною одиницею Active Directory (ОП). Якщо користувачі вже ввійшли до SharePoint, а потім переміщуються до іншого підрозділу та повторно з SharePoint, вони можуть виникати з цієї проблеми.

1. Щоб вирішити цю проблему, слід відновити початковий UPN, з кроками у статті, [відновити користувача в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Якщо не вдається відновити вихідний користувач слід видалити старого користувача з OneDrive сайту, за допомогою цих дій, [видалення користувача з відомості про користувача списку](). 
3. Після цього, ви можете перевірити, користувач має права адміністратора на OneDrive сайт, виконавши дії, щоб [Додати адміністратора для користувача onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Докладніші відомості про рівні дозволів наведено в статті, які [розуміють рівні дозволів у програмі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
