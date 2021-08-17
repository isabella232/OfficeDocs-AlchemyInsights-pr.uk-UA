---
title: Увімкнення Сейф вкладень для SharePoint Online, OneDrive та Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894484"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнення Сейф вкладень для SharePoint Online, OneDrive та Microsoft Teams

1. Використовуючи облікові дані глобального адміністратора або адміністратора безпеки, відкрийте портал Microsoft 365 Defender на сторінці , а потім у розділі Політики & політики загроз <https://security.microsoft.com>  \>  \> **Сейф вкладення**  в розділі Політики

   Щоб перейти безпосередньо на **Сейф Вкладення,** <https://security.microsoft.com/safeattachmentv2> скористайтеся .

2. На сторінці **Сейф вкладення натисніть** кнопку **Глобальні параметри.**
3. На виліту, що з'явиться, виберіть Увімкнути Захисник Microsoft для Office 365 для **SharePoint, OneDrive і Microsoft Teams**, а потім натисніть кнопку **Зберегти**.

    > [!TIP]
    >
    > Щоб покращити захист вкладень для Сейф, SharePoint, OneDrive та інших Microsoft Teams, виконайте такі Microsoft Teams:
    >
    > - Щоб заборонити користувачам завантажувати зловмисні файли, використовуйте значення параметра `$true` *DisallowInfectedFileDownload* в командлеті **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** у SharePoint Online PowerShell. Докладні відомості див. в SharePoint Online PowerShell, щоб заборонити користувачам завантажувати [зловмисні файли.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Створення політики оповіщення для виявлених файлів](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Докладні відомості [див. в Сейф. в Office 365, SharePoint, OneDrive та Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
