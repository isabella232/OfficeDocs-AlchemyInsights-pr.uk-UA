---
title: Увімкнути АТФ Office 365 для SharePoint, OneDrive і Microsoft команд
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403054"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнути Office 365 передові загроза захист для SharePoint онлайн, OneDrive і Microsoft команд

1. Перейти до https://protection.office.com та виконайте вхід.
2. Вибрати **загрозу управління** > **політика** > **Безпечний вкладення**.
3. Виберіть **Увімкнути АТФ для SharePoint, OneDrive та команди Microsoft**і натисніть кнопку **зберегти**.
4. (Рекомендовано) Як глобальна адміністратора або адміністратор SharePoint Online запустити командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) із параметром **DisallowInfectedFileDownload** , встановіть значення *true*.
5. (Рекомендовано) [Настроювання оповіщень](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) на виявлені файли.

> [!NOTE]
> АТФ буде НТО сканування кожен окремий файл у SharePoint Online, OneDrive або Microsoft команд. Перевіряються при асинхронно, через процес, який використовує обміну і гостьова події діяльності, поряд з smart евристики і загроза сигнали для ідентифікації шкідливі файли. Див [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).