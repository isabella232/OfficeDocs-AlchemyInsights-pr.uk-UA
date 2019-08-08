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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Усунення несправностей доступ заборонено повідомлень до OneDrive для бізнес сайтів

Ця проблема найчастіше виникає, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID. Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП). Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.

1. Для вирішення цієї проблеми слід відновити оригінальний УПН з дії, зазначені в статті,[відновити користувача у службі Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Якщо не вдалося відновити оригінальний користувача слід видалити старі користувача з сайту OneDrive, за допомогою цих кроків, [Видалити користувача зі списку відомостей про користувача](). 
3. Після того, як це буде зроблено, ви можете перевірити, користувач має права адміністратора на сайті OneDrive, виконавши кроки, щоб [Додати адміністратор в для користувача OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Для отримання додаткової інформації на рівні дозволів перегляньте статтю, [розуміння рівнів дозволів в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
