---
title: Оповіщення сповіщень SharePoint не доставлено
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751264"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Оповіщення сповіщень SharePoint не доставлено

Перевірте папку "НЕБАЖАНА пошта" в електронному листі, оскільки іноді оповіщення можуть перейти туди.

Визначити, чи не доставлено **всі оповіщення** , або якщо не доставляється **окреме оповіщення** з певного файлу або бібліотеки.

- **Окремі оповіщення не доставляються**: якщо не доставлено окреме оповіщення з певного файлу або бібліотеки, ви можете спробувати видалити та відтворити його повторно. У статті [керування, перегляд і видалення оповіщень SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) для повторного створення оповіщення.
- **Усі оповіщення не доставляються**: якщо не доставлено всі оповіщення з кількох файлів або бібліотек, перейдіть на [приладну дошку справність служби](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб перевірити всі рекомендації та інциденти, що можуть виникнути в службі SharePoint або Exchange. Ця проблема може бути з функцією оповіщення служби SharePoint або затримками в повідомленнях електронної пошти за допомогою Exchange. Також слід пам'ятати про те, чи доставлятимуться інші повідомлення електронної пошти, а якщо це можливо, проблема з затримкою Exchange.

Запитання й відповіді про оповіщення:

- Не можна передавати оповіщення до групи розсилки, підтримуються лише групи безпеки та O365.
- Не можна настроювати шаблони сповіщень електронної пошти; щоб досягти цих потреб, потрібно скористатися робочим циклом Microsoft FLOW або конструктора SharePoint Designer.

## <a name="related-topics"></a>Пов'язані теми

Хочете спробувати Microsoft Flow у службі SharePoint Online?

- [Створення потоку](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint і передавання](https://flow.microsoft.com//blog/sharepoint-and-flow/)
