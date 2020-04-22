---
title: Усунення несправностей у доступі повідомлення
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758544"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Виправлення неполадок із Забороними доступом у центрі адміністрування SharePoint/OneDrive

Якщо ви отримуєте повідомлення про відмову в доступі під час спроби перейти до центру адміністрування SharePoint/OneDrive, будь ласка, переконайтеся, що ви [призначаєте ліцензію користувачу](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Якщо користувач має ліцензію, ви також повинні переконатися, що вони [призначені роль адміністратора](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , які можуть отримати доступ до центрів адміністрування.

Ця проблема також може виникати, коли користувач видаляється і повторно створюється з одного учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (унікальний ІДЕНТИФІКАТОР паспорта) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний PUID. Другий сценарій передбачає синхронізацію каталогів із організаційною одиницею Active Directory (ОП). Якщо користувачі вже ввійшли до SharePoint, а потім переміщуються до іншого підрозділу та повторно з SharePoint, вони можуть виникати з цієї проблеми.

Щоб вирішити цю проблему, слід відновити початковий UPN, виконавши дії, описані в статті, [відновити користувача в Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Примітка: Якщо Центр адміністрування OneDrive або SharePoint недоступний для кількох користувачів, які раніше мали доступ, може виникнути проблема з тимчасовим обслуговуванням.  [Перегляньте приладну дошку справності служб](https://portal.office.com/adminportal/home#/servicehealth).


