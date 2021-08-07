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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998821"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Помилки синхронізації через повторювані об'єкти

Після завершення синхронізації служби каталогів у програмі Outlook може з'явитися одне з таких повідомлень про Microsoft 365:

- Не вдалося оновити цей об'єкт у службах Microsoft Online Services, тому що наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які можуть бути вже пов'язані з іншим об'єктом у локальному каталозі.

- Синхронізований об'єкт із тією ж адресою проксі-сервера вже існує в каталозі служб Microsoft Online Services.

- Не вдається оновити цей об'єкт, оскільки такі атрибути, пов'язані з цим об'єктом, уже можуть бути пов'язані з іншим об'єктом у службах локального каталогу (UserPrincipalName).

Щоб визначити та вирішити цю проблему, завантажте й запустіть засіб виправлення помилок [IdFix DirSync.](https://github.com/Microsoft/idfix)

Докладні відомості див. [в статті KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
