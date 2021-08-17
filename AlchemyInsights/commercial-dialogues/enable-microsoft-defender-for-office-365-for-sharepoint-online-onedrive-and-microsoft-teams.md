---
title: Увімкнення Microsoft Defender для Office 365 для SharePoint Online, OneDrive та Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058887"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнення Microsoft Defender для Office 365 для SharePoint Online, OneDrive та Microsoft Teams

1. Увійдіть у Центр безпеки та відповідності за допомогою облікових даних глобального адміністратора або [адміністратора Office 365 безпеки та відповідності.](https://protection.office.com/)
2. В **області ліворуч** виберіть Керування загрозами, а потім **– Політика** Сейф  >  [вкладення.](https://protection.office.com/safeattachment)
3. Установіть **прапорець Увімкнути Захисник Microsoft Office 365 для SharePoint, OneDrive і Microsoft Teams**, а потім натисніть кнопку **Зберегти**.
    > [!TIP]
    >
    > - Якщо ви глобальний адміністратор або адміністратор служби SharePoint Online, запустіть цей командлет PowerShell із параметром **DisallowInfectedFileDownload,** для яких установлено значення *true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Настроювання оповіщень про виявлені файли](https://go.microsoft.com/fwlink/?linkid=2092110)

Докладні відомості див. в [статті Захисник Microsoft Office 365 для SharePoint, OneDrive і Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
