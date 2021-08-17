---
title: Усунення несправностей, пов'язаних із повідомленнями про від'їд
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085249"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Усунення несправностей, пов'язаних із повідомленнями про від'OneDrive Access у Sharepoint або OneDrive адміністрування

Якщо ви отримуєте повідомлення про відхилення доступу під час спроби перейти до Центру адміністрування Sharepoint або OneDrive, переконайтеся, що ви призначили [ліцензію користувачу.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Якщо користувач має ліцензію, слід [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) також переконатися, що їм призначено роль адміністратора, яка має доступ до Центрів адміністрування.

Ця проблема також може виникати, коли користувач видаляється та повторно створюється з таким самим іменем учасника-користувача (UPN). Новий обліковий запис створюється за допомогою іншого значення PUID (Passport Unique ID). Коли користувач намагається отримати доступ до колекції сайтів або OneDrive, у користувача є неправильний ідентифікатор PUID. Другий сценарій передбачає синхронізацію служби каталогів з підрозділом організації Active Directory. Якщо користувачі вже ввійшли в SharePoint, а потім переміщуються до іншого єдиного входу та повторно SharePoint, у них може виникнути ця проблема.

Щоб вирішити цю проблему, слід відновити початкове ім'я UPN, доки не буде вирішено кроки, описані в статті Відновлення користувача [в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Примітка. Якщо Центр адміністрування OneDrive або SharePoint недоступний для кількох користувачів, які раніше мали доступ, можуть видавитися тимчасова проблема з обслуговуванням.  [Перевірте приладну дошку справності служби.](https://portal.office.com/adminportal/home#/servicehealth)


