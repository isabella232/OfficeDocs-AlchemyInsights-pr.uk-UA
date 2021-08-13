---
title: Виправлення неполадок, пов'язаних із повідомленнями про OneDrive для бізнесу доступу
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957814"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Виправлення неполадок, пов'язаних із повідомленнями про OneDrive для бізнесу доступу

Найчастіше ця проблема виникає, коли користувач видаляється та повторно створюється з іменем учасника-користувача (UPN). Новий обліковий запис створюється за допомогою іншого значення PUID (Passport Unique ID). Коли користувач намагається отримати доступ до колекції сайтів або OneDrive, у користувача є неправильний ідентифікатор PUID. Другий сценарій передбачає синхронізацію служби каталогів з підрозділом організації Active Directory. Якщо користувачі вже ввійшли в SharePoint, а потім переміщуються до іншого єдиного входу та повторно SharePoint, у них може виникнути ця проблема.

1. Щоб вирішити цю проблему, потрібно відновити вихідне ім'я UPN, як описано в статті Відновлення [користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Якщо не вдається відновити вихідного користувача, старого користувача слід видалити із сайту OneDrive, додавши наведені нижче дії, видаліть користувача зі списку [відомостей про користувача.]() 
3. Після цього можна перевірити, чи має користувач права адміністратора на сайт OneDrive, виконавши вказівки з додавання адміністратора для облікового [запису OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Докладні відомості про рівні дозволів див. в статті Докладні відомості про рівні дозволів у [SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
