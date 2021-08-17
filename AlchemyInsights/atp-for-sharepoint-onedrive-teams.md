---
title: Microsoft Defender для Office 365 для SharePoint, OneDrive та інших Microsoft Teams
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
ms.openlocfilehash: 0d0fff3e699d46af2a19a8ad60696b824bafa109
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314983"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender для Office 365 для SharePoint, OneDrive та інших Microsoft Teams

Щоб активувати Захисник Microsoft для Office 365, виконайте такі Office 365:

1. Перейдіть до облікового запису глобального адміністратора або адміністратора безпеки та [https://protection.office.com](https://protection.office.com) ввійдіть у неї.

2. В області переходів ліворуч у **розділі Керування загрозами** виберіть **політика** \> **Сейф вкладення.**

3. Виберіть **Увімкнути Захисник для Office 365 для SharePoint, OneDrive і Microsoft Teams**.

4. [Створіть політику оповіщення про](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) дії, щоб отримувати сповіщення про виявлення зловмисних файлів.

Докладні вказівки наведено в статті Увімкнення Сейф вкладень для [SharePoint, OneDrive та інших Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Примітка.** За дизайном Microsoft Defender для Office 365 не сканує кожен окремий файл у SharePoint Online, OneDrive для бізнесу або Microsoft Teams. Файли асинхронно скануються процесом, який використовує дії з надання спільного доступу, гостьові дії та сигнали загроз для виявлення зловмисних файлів. Докладні відомості [див. в Сейф. в SharePoint, OneDrive та Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
