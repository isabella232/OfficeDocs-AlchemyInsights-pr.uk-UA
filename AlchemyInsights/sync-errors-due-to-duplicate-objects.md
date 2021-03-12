---
title: 902 (помилки синхронізації через повторювані об'єкти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708083"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Помилки синхронізації через повторювані об'єкти

Після завершення синхронізації служби каталогів у Microsoft 365 може з'явитися одне з таких повідомлень про помилку:

- Не вдалося оновити цей об'єкт у службах Microsoft Online Services, оскільки наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які вже можуть бути пов'язані з іншим об'єктом у локальному каталозі.

- Синхронізований об'єкт із тією самою адресою проксі-сервера, що вже існує в каталозі служб Microsoft Online Services.

- Не вдалося оновити цей об'єкт, оскільки наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які вже можуть бути пов'язані з іншим об'єктом у службах локальної служби каталогів: UserPrincipalName.

Щоб визначити та вирішити цю проблему, завантажте та запустіть [засіб виправлення помилок Idfix DirSync](https://github.com/Microsoft/idfix).

Щоб отримати докладніші відомості, ознайомтеся з [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
