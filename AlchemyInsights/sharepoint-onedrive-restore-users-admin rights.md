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
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511205"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Виправлення неполадок, які заборонено доступ до повідомлень OneDrive, для бізнес-сайтів

Ця проблема найчастіше виникає, коли користувач видаляється і повторно створюється з одного учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (унікальний ІДЕНТИФІКАТОР паспорта) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний PUID. Другий сценарій передбачає синхронізацію каталогів із організаційною одиницею Active Directory (ОП). Якщо користувачі вже ввійшли до SharePoint, а потім переміщуються до іншого підрозділу та повторно з SharePoint, вони можуть виникати з цієї проблеми.

1. Щоб вирішити цю проблему, слід відновити початковий UPN, з кроками у статті, [відновити користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Якщо не вдається відновити вихідний користувач слід видалити старого користувача з OneDrive сайту, за допомогою цих дій, [видалення користувача з відомості про користувача списку](). 
3. Після цього, ви можете перевірити, користувач має права адміністратора на OneDrive сайт, виконавши дії, щоб [Додати адміністратора для користувача onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Докладніші відомості про рівні дозволів наведено в статті, які [розуміють рівні дозволів у програмі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
