---
title: Виправлення неполадок із відхилень у програмі Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767684"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Виправлення неполадок із Заперечуванням повідомлень у центрі адміністрування SharePoint або OneDrive

Якщо ви отримуєте повідомлення про відмову в доступі під час спроби перейти до центру адміністрування SharePoint або OneDrive, переконайтеся, що ви [призначите ліцензію користувачу](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Якщо користувач має ліцензію, слід також переконатися, що їм [призначено роль адміністратора](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , які можуть отримати доступ до центрів адміністрування.

Ця проблема також може виникати, коли користувач видаляється та повторно створюється за допомогою одного імені учасника-користувача (UPN). Новий обліковий запис створюється за допомогою іншого значення "PUID" (унікальний ІДЕНТИФІКАТОР паспорта). Коли користувач спробує отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний ідентифікатор. Другий сценарій передбачає синхронізацію служби каталогів за допомогою організаційної одиниці Active Directory (OU). Якщо користувачі вже ввійшли у службу SharePoint, а потім переміщуються до іншої програми SharePoint, вони можуть виникнути під час цієї проблеми.

Щоб вирішити цю проблему, потрібно відновити початковий УПН, виконавши кроки, описані в статті, [відновлення користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Примітка. Якщо Центр адміністрування Onedriveабо SharePoint недоступний для кількох користувачів, які раніше мали доступ, може виникнути тимчасова проблема служби.  [Перевірте приладну дошку справності служби](https://portal.office.com/adminportal/home#/servicehealth).


