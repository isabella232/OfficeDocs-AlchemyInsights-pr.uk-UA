---
title: Захисник Microsoft Office 365 для SharePoint, OneDrive та Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: c42786559d527a5ef9a0a8cfad1476f4d122b6d5570ca5b9ea138b21a153ae96
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896356"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Захисник Microsoft Office 365 для SharePoint, OneDrive та Microsoft Teams

Щоб активувати Захисник Microsoft для Office 365, виконайте наведені нижче Office 365.

1. Перейдіть до облікового запису глобального адміністратора або адміністратора безпеки та [https://protection.office.com](https://protection.office.com) ввійдіть у неї.

2. В області переходів ліворуч у **розділі Керування загрозами** виберіть **політика** \> **Сейф вкладення.**

3. Виберіть **Увімкнути Захисник для Office 365 для SharePoint, OneDrive і Microsoft Teams**.

4. [Створіть політику оповіщення про](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) дії, щоб отримувати сповіщення про виявлення зловмисних файлів.

Докладні вказівки наведено в статті Увімкнення Сейф вкладень для [SharePoint, OneDrive і Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Примітка.** За дизайном Microsoft Defender для Office 365 не сканує кожен окремий файл у SharePoint Online, OneDrive для бізнесу або Microsoft Teams. Файли асинхронно скануються процесом, який використовує дії з надання спільного доступу, гостьові дії та сигнали загроз для виявлення зловмисних файлів. Докладні відомості [див. в Сейф Вкладення для SharePoint, OneDrive та Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
