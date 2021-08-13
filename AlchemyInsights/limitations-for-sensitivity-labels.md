---
title: Обмеження чутливості підписів для Office файлів у SharePoint і OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813170"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Обмеження чутливості підписів для Office файлів у SharePoint і OneDrive

У разі ввімкнення підписів чутливості для Office файлів у SharePoint і OneDrive слід врахувати вимоги та обмеження, до яких належать:

- SharePoint і OneDrive не вдається обробити деякі файли, позначені та зашифровані з класичних програм Office, коли файли містять дані PowerQuery, дані, збережені спеціальними надбудовами або настроюваними частинами XML.
- SharePoint і OneDrive не застосовувати підписи чутливості автоматично до наявних файлів, уже зашифрованих за допомогою підписів Azure Information Protection (AIP). Щоб застосувати підписи чутливості до зашифрованих файлів: 
    - Переконайтеся, що етикетки AIP перенесено та опубліковано в Центрі Microsoft 365 відповідності.
    - Завантажте файли з підписами, а потім передайте їх у вихідне розташування SharePoint або OneDrive розташування.
- Для зашифрованих документів друк не підтримується.

Докладні відомості про обмеження див. в Office та SharePoint [OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
