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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332400"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Увімкнення Сейф вкладень для SharePoint Online, OneDrive та Microsoft Teams

1. Використовуючи облікові дані глобального адміністратора або адміністратора безпеки, відкрийте портал Microsoft 365 Defender на сторінці , а потім у розділі Політики & політики загроз <https://security.microsoft.com>  \>  \> **Сейф Вкладення**  в розділі Політики

   Щоб перейти безпосередньо на **Сейф Вкладення,** <https://security.microsoft.com/safeattachmentv2> скористайтеся .

2. На сторінці **Сейф вкладення** натисніть кнопку **Глобальні параметри.**
3. На виліту, що з'явиться, виберіть увімкнути Захисник Microsoft Office 365 для **SharePoint, OneDrive і Microsoft Teams**, а потім натисніть кнопку **Зберегти**.

    **Порада.** Щоб підвищити захист вкладень Сейф для користувачів SharePoint, OneDrive, виконайте наведені нижче дії, щоб Microsoft Teams.
    - Щоб заборонити користувачам завантажувати зловмисні файли, використовуйте значення параметра `$true` *DisallowInfectedFileDownload* в командлеті **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** у SharePoint Online PowerShell. Докладні відомості див. в SharePoint Online PowerShell, щоб заборонити користувачам завантажувати [зловмисні файли.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Створення політики оповіщення для виявлених файлів](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Докладні відомості [див. в Сейф.](https://go.microsoft.com/fwlink/?linkid=2092041)в Office 365 відомості про SharePoint, OneDrive та Microsoft Teams .
