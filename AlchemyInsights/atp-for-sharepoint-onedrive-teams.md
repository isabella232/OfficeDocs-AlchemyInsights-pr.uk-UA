---
title: АТФ для SharePoint, OneDrive і Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508433"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>АТФ для SharePoint, OneDrive і Microsoft teams

Щоб увімкнути розширений захист від загроз, виконайте наведені нижче дії.

1. Перейдіть до [https://protection.office.com](https://protection.office.com) і ввійдіть за допомогою глобального адміністратора або облікового запису адміністратора безпеки.

2. В області переходів ліворуч у розділі **керування загрозами**виберіть **політики** \> **безпечні вкладення**.

3. Виберіть **Увімкнути АТФ для SharePoint, OneDrive і Microsoft teams**.

4. [Створення політики оповіщення про активність](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) для отримання сповіщень під час виявлення зловмисних файлів.

Докладні інструкції наведено в цій [темі](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Примітка**: за ДИЗАЙНОМ, АТФ не сканує кожен файл у SharePoint Online, OneDrive для бізнесу або Microsoft teams. Файли скануються асинхронно процесом, який використовує спільну діяльність, гостьовій активності та сигнали загрози для ідентифікації шкідливих файлів. Докладніші відомості наведено в цій [статті](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
