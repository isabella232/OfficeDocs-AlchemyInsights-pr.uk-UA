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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737362"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Помилки синхронізації через повторювані об'єкти

Після завершення синхронізації служби каталогів у Microsoft 365 може з'явитися одне з таких повідомлень про помилку:

- Не вдалося оновити цей об'єкт у службах Microsoft Online Services, оскільки наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які вже можуть бути пов'язані з іншим об'єктом у локальному каталозі.

- Синхронізований об'єкт із тією самою адресою проксі-сервера, що вже існує в каталозі служб Microsoft Online Services.

- Не вдалося оновити цей об'єкт, оскільки наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які вже можуть бути пов'язані з іншим об'єктом у службах локальної служби каталогів: UserPrincipalName.

Щоб визначити та вирішити цю проблему, завантажте та запустіть [засіб виправлення помилок Idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Щоб отримати докладніші відомості, ознайомтеся з [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
