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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707975"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Виправлення неполадок із Заперечуванням повідомлень у центрі адміністрування SharePoint або OneDrive

Якщо ви отримуєте повідомлення про відмову в доступі під час спроби перейти до центру адміністрування SharePoint або OneDrive, переконайтеся, що ви [призначите ліцензію користувачу](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Якщо користувач має ліцензію, слід також переконатися, що їм [призначено роль адміністратора](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , які можуть отримати доступ до центрів адміністрування.

Ця проблема також може виникати, коли користувач видаляється та повторно створюється за допомогою одного імені учасника-користувача (UPN). Новий обліковий запис створюється за допомогою іншого значення "PUID" (унікальний ІДЕНТИФІКАТОР паспорта). Коли користувач спробує отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильний ідентифікатор. Другий сценарій передбачає синхронізацію служби каталогів за допомогою організаційної одиниці Active Directory (OU). Якщо користувачі вже ввійшли у службу SharePoint, а потім переміщуються до іншої програми SharePoint, вони можуть виникнути під час цієї проблеми.

Щоб вирішити цю проблему, потрібно відновити початковий УПН, виконавши кроки, описані в статті, [відновлення користувача в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Примітка. Якщо Центр адміністрування Onedriveабо SharePoint недоступний для кількох користувачів, які раніше мали доступ, може виникнути тимчасова проблема служби.  [Перевірте приладну дошку справності служби](https://portal.office.com/adminportal/home#/servicehealth).


