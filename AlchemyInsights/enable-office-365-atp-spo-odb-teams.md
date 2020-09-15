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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709928"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнення захисту від розширених загроз в Office 365 для служби SharePoint Online, OneDrive і команд Microsoft

1. Перейдіть на сторінку https://protection.office.com та ввійдіть.
2. Виберіть **Threat management**пункт  >  **Policy**  >  **безпечні вкладення**політики керування загрозою.
3. Виберіть **Увімкнути АТФ для SharePoint, OneDrive і команд Microsoft**, а потім натисніть кнопку **зберегти**.
4. Рекомендовані Як Глобальний адміністратор або адміністратор служби SharePoint Online запустіть командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) за допомогою параметра **DisallowInfectedFileDownload** (значення *True*).
5. Рекомендовані [Настроювання оповіщень](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.

> [!NOTE]
> АТФ буде nЩоб сканувати кожен файл у службі SharePoint Online, OneDrive або Microsoft. Файли, відскановані в асинхронному режимі, за допомогою процесу, який використовує події спільного доступу та дії гостей, а також розумні евристики та сигнали загроз для ідентифікації зловмисних файлів. Переглянути [АТФ для SharePoint, OneDrive і команд Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).