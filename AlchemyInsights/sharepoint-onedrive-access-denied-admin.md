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
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716667"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Усунення проблем: відмовлено у доступі до повідомлення центру адміністрування Sharepoint/OneDrive

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Якщо ви отримуєте в доступі повідомлення при спробі перейдіть до центру адміністрування Sharepoint/OneDrive, будь ласка переконайтесь, що ви <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">призначите ліцензію для користувача </a>. Якщо користувач має ліцензію, ви повинні також переконайтеся, що вони <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">призначені роль адміністратора</a> доступ адміністратора центрів.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Ця проблема також може виникнути, коли користувач видаляється та створюється повторно з ж ім'я учасника-користувача (UPN). Новий обліковий запис створюється за допомогою різних PUID (паспорта-унікальний Ідентифікатор) значення. Коли користувач намагається отримати доступ до колекції сайтів або їх OneDrive, користувач має неправильну PUID. Другий сценарій передбачає синхронізації каталогів з Active Directory організаційного підрозділу (ОП). Якщо користувачі мають вже увійшли до SharePoint і потім переїхав до різних OU і resynced з SharePoint, вони можуть відчувати цю проблему.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Щоб вирішити цю проблему, слід відновити оригінальний УПН з дії, зазначені в статті, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">відновити користувача у службі Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Примітка:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">Якщо OneDrive або адміністратор SharePoint центр недоступна для декількох користувачів, які раніше мали доступ, це може бути тимчасова служби питання.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Перевірити службу здоров'я dashboard</span></a>.</span></em></span></span></p>


