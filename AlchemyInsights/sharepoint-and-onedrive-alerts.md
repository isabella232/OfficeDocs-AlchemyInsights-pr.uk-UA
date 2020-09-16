---
title: Затримки в отриманні сповіщень SharePoint і OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727264"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Затримки в отриманні сповіщень SharePoint і OneDrive

- Спочатку перевірте папку "Небажана пошта" або "спам" у повідомленні електронної пошти.
- Якщо **всі оповіщення з кількох файлів або бібліотек затримуються**, перейдіть на [приладну дошку справність служби](https://portal.office.com/adminportal/home?ref=/servicehealth) , щоб перевірити наявність будь-яких інших або інцидентів, які можуть виникнути в службі SharePoint або Exchange. Ця проблема може бути з функцією оповіщення служби SharePoint або затримками в повідомленнях електронної пошти за допомогою Exchange. Зверніть увагу, чи доставлятимуться інші повідомлення електронної пошти (якщо ні, то проблема може бути затримка Exchange).
- Якщо **окреме оповіщення з певного файлу або бібліотеки не доставлено**, спробуйте видалити та відтворити його повторно. У статті [керування, перегляд і видалення оповіщень SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) для повторного створення оповіщення.

> [!NOTE]
> - Оповіщення не можна надіслати до групи розсилки. Підтримуються лише групи безпеки та O365.
> - Ви не можете настроювати шаблони сповіщень електронної пошти. Щоб досягти цих документів, потрібно скористатися робочим циклом Microsoft Flow або конструктора SharePoint Designer.
