---
title: Увімкнення Office 365 РЗЗ для SharePoint, OneDrive та Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332180"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнення Microsoft Defender для Office 365 для SharePoint Online, OneDrive та Microsoft Teams

1. Перейдіть до входу https://protection.office.com та ввійдіть.
2. Виберіть **Політика керування**  >    >  **загрозами Сейф вкладеннях.**
3. Установіть **прапорець Увімкнути Захисник для Office 365 для SharePoint, OneDrive і Microsoft Teams**, а потім натисніть кнопку **Зберегти**.
4. (Рекомендовано) Якщо ви глобальний адміністратор або адміністратор служби SharePoint Online, запустіть командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) із для параметра **DisallowInfectedFileDownload** значення *TRUE.*
5. (Рекомендовано) [Настроювання оповіщень](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) про виявлені файли.

**Примітка.** Microsoft Defender для Office 365 не скануватиме кожен окремий файл у SharePoint Online, OneDrive або Microsoft Teams. Файли скануються асинхронно через процес, який використовує події для надання спільного доступу та гостьових дій, а також інтелектуальну евристіку та сигнали загроз для виявлення зловмисних файлів. Докладні [відомості див. в статті Захисник Microsoft Office 365 для SharePoint, OneDrive і Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
