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
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Надати користувачам доступ до SharePoint і OneDrive

Ця проблема найчастіше виникає, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID. Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП). Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.

Для вирішення цієї проблеми слід відновити оригінальний УПН з дії, зазначені в статті,[відновити користувача у службі Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

Після того, як це буде зроблено, ви можете перевірити, користувач має права адміністратора на сайті OneDrive, виконавши кроки, щоб [Додати адміністратор в для користувача OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Для отримання додаткової інформації на рівні дозволів перегляньте статтю, [розуміння рівнів дозволів в SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
