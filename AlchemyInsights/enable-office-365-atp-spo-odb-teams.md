---
title: Увімкнення АТФ Office 365 для SharePoint, OneDrive та команд Microsoft
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801096"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Активація програми Microsoft Defender для Office 365 для SharePoint Online, OneDrive та команд Microsoft

1. Перейдіть на сторінку https://protection.office.com та ввійдіть.
2. Виберіть **Threat management** пункт  >  **Policy**  >  **безпечні вкладення** політики керування загрозою.
3. Виберіть **Увімкнути АТФ для SharePoint, OneDrive і команд Microsoft** , а потім натисніть кнопку **зберегти** .
4. Рекомендовані Як Глобальний адміністратор або адміністратор служби SharePoint Online запустіть командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) за допомогою параметра **DisallowInfectedFileDownload** (значення *True* ).
5. Рекомендовані [Настроювання оповіщень](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.

> [!NOTE]
> АТФ буде nЩоб сканувати кожен файл у службі SharePoint Online, OneDrive або Microsoft. Файли, відскановані в асинхронному режимі, за допомогою процесу, який використовує події спільного доступу та дії гостей, а також розумні евристики та сигнали загроз для ідентифікації зловмисних файлів. Переглянути [АТФ для SharePoint, OneDrive і команд Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).