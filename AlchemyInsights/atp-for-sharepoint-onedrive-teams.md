---
title: "\"АТФ для SharePoint\", \"OneDrive\" і груп Microsoft"
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715582"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>"АТФ для SharePoint", "OneDrive" і груп Microsoft

Виконайте наведені нижче дії, щоб активувати розширений захист від загроз:

1. Перейдіть на сторінку [https://protection.office.com](https://protection.office.com) та увійдіть за допомогою облікового запису глобального адміністратора або адміністратора безпеки.

2. В області переходів ліворуч у розділі **керування загрозою**виберіть команду **Policy** \> **надійні вкладення**політики.

3. Виберіть **Увімкнути АТФ для SharePoint, OneDrive і команд Microsoft**.

4. [Створіть політику оповіщення про дії,](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) щоб отримувати сповіщення, коли ми Виявляйте зловмисними файлами.

Щоб отримати докладні вказівки, ознайомтеся з цією [темою](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Примітка**: за конструкцією АТФ не перевіряє кожний файл у службі SharePoint Online, OneDrive для бізнесу або команд Microsoft. Файли буде перевірено в асинхронному процесі, за допомогою якого ви надаєте спільний доступ до дій, гостьової діяльності та сигналів загрози для ідентифікації зловмисних файлів. Щоб отримати докладніші відомості, ознайомтеся з цією [темою](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
