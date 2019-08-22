---
title: 'Усунення проблем: відмовлено у доступі до повідомлення'
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503566"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Усунення проблем: відмовлено у доступі до повідомлення центру адміністрування Sharepoint/OneDrive

Якщо ви отримуєте в доступі повідомлення при спробі перейдіть до центру адміністрування Sharepoint/OneDrive, будь ласка переконайтесь, що ви [призначите ліцензію для користувача](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Якщо користувач має ліцензію, ви повинні також переконайтеся, що вони [призначені роль адміністратора](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) доступ адміністратора центрів.

Ця проблема також може виникнути, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID. Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП). Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.

Щоб вирішити цю проблему, слід відновити оригінальний УПН з дії, зазначені в статті, [відновити користувача у службі Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Примітка: Якщо OneDrive або адміністратор SharePoint центр недоступна для декількох користувачів, які раніше мали доступ, це може бути тимчасова служби питання.  [Перевірте службу здоров'я приладної дошки](https://portal.office.com/adminportal/home#/servicehealth).


