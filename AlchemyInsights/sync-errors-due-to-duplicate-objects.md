---
title: 902 (помилки синхронізації через повторювані об'єкти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767162"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Помилки синхронізації через повторювані об'єкти

Може з'явитися одне з таких повідомлень про помилку під час синхронізації каталогів, що закінчується в Microsoft 365:

- Не вдалося оновити цей об'єкт у службах Microsoft Online, оскільки такі атрибути, пов'язані з цим об'єктом, мають значення, які можуть бути вже пов'язані з іншим об'єктом у локальному каталозі.

- Синхронізований об'єкт з однаковою проксі-адресою вже існує у вашому каталозі служб Microsoft Online Services.

- Не вдалося оновити цей об'єкт, оскільки такі атрибути, пов'язані з цим об'єктом, мають значення, які можуть бути вже пов'язані з іншим об'єктом у службах локальних каталогів: ім'я користувача.

Щоб визначити та вирішити цю проблему, завантажте та запустіть [засіб виправлення помилок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Для отримання додаткових відомостей див. [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
