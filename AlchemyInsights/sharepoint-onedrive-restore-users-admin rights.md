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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Виправлення неполадок із відхилень у програмі Access для веб-сайтів у службі OneDrive

Ця проблема найчастіше виникає, коли користувач видаляється та повторно створюється за допомогою одного імені учасника-користувача (UPN). Новий обліковий запис створюється за допомогою іншого значення "PUID" (унікальний ІДЕНТИФІКАТОР паспорта). Коли користувач спробує отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний ідентифікатор. Другий сценарій передбачає синхронізацію служби каталогів за допомогою організаційної одиниці Active Directory (OU). Якщо користувачі вже ввійшли у службу SharePoint, а потім переміщуються до іншої програми SharePoint, вони можуть виникнути під час цієї проблеми.

1. Щоб вирішити цю проблему, потрібно відновити початковий UPN, виконавши кроки, описані в статті, [відновлення користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Якщо ви не можете відновити початковий користувач, який ви маєте видалити старий користувач із сайту OneDrive, виконавши наведені нижче дії, [видаліть користувача зі списку відомостей про користувача](). 
3. Після цього ви можете перевірити, чи користувач має права адміністратора на веб-сайт OneDrive, виконавши вказівки з [Додавання адміністратора для onedrive користувача](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Докладні відомості про рівні дозволів наведено в статті, [розумінні рівнів дозволів у службі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
