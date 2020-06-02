---
title: Увімкнення АТФ для Office 365 для SharePoint, OneDrive і Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506939"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнути розширений захист від загроз Office 365 для SharePoint Online, OneDrive і Microsoft teams

1. Перейдіть до https://protection.office.com входу та ввійдіть.
2. Виберіть **Threat management**  >  **Policy**  >  **безпечне вкладення**політики керування загрозами.
3. Виберіть **Увімкнути АТФ для SharePoint, OneDrive і Microsoft teams**і натисніть кнопку **зберегти**.
4. Рекомендується Як Глобальний адміністратор або адміністратор SharePoint Online, запустити командлет [Set-Споживнент](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) з параметром **DisallowInfectedFileDownload** , встановлений на *True*.
5. Рекомендується [Налаштуйте оповіщення](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.

> [!NOTE]
> АТФ буде НТО сканувати кожен файл у SharePoint Online, OneDrive або Microsoft teams. Файли скануються асинхронно через процес, який використовує події спільного використання та гостьової активності, а також смарт-евристики та сигнали загрози для ідентифікації шкідливих файлів. Дивіться [АТФ для SharePoint, OneDrive і Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).