---
title: Затримки в отриманні сповіщень SharePoint і OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785686"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Затримки в отриманні сповіщень SharePoint і OneDrive

- Спочатку перевірте папку "Небажана пошта" або "спам" у повідомленні електронної пошти.
- Якщо **всі оповіщення з кількох файлів або бібліотек затримуються**, перейдіть на [приладну дошку справність служби](https://portal.office.com/adminportal/home?ref=/servicehealth) , щоб перевірити наявність будь-яких інших або інцидентів, які можуть виникнути в службі SharePoint або Exchange. Ця проблема може бути з функцією оповіщення служби SharePoint або затримками в повідомленнях електронної пошти за допомогою Exchange. Зверніть увагу, чи доставлятимуться інші повідомлення електронної пошти (якщо ні, то проблема може бути затримка Exchange).
- Якщо **окреме оповіщення з певного файлу або бібліотеки не доставлено**, спробуйте видалити та відтворити його повторно. У статті [керування, перегляд і видалення оповіщень SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) для повторного створення оповіщення.

> [!NOTE]
> - Оповіщення не можна надіслати до групи розсилки. Підтримуються лише групи безпеки та O365.
> - Ви не можете настроювати шаблони сповіщень електронної пошти. Щоб досягти цих документів, потрібно скористатися робочим циклом Microsoft Flow або конструктора SharePoint Designer.
