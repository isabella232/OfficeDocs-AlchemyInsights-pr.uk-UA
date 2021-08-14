---
title: Вирішення Teams помилки входу AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953062"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Вирішення Teams помилки входу AADSTS9000411

Під час входу в Microsoft Teams може з'явитися повідомлення про помилку: На жаль, у нас виникли проблеми з входом **у AADSTS9000411. Запит відформатовано неправильно. Буде дубльовано login_hint параметр.**

Щоб вирішити цю проблему, переконайтеся, що Microsoft Teams клієнтів оновлено. Докладні відомості про оновлення клієнта див. в [Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Якщо з якоїсь причини не вдається оновити клієнт, буде очищено більшість кешованих даних. Однак якщо після виходу або входу проблеми не зникнуть, закрийте Teams та очистіть кеш клієнта, виконавши такі дії:
1. Закрийте Microsoft Teams.
2. Перейдіть до папки: %appdata%\microsoft\teams і видаліть усі файли.
3. Знову Microsoft Teams.
