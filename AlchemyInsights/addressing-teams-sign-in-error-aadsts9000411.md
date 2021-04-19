---
title: Помилка входу в Teams AADSTS9000411
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
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822008"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Помилка входу в Teams AADSTS9000411

Під час входу в Microsoft Teams може з'явитися повідомлення про помилку: На жаль, у нас виникли проблеми з входом **у AADSTS9000411. Запит відформатовано неправильно. Буде дубльовано login_hint параметр.**

Щоб вирішити цю проблему, переконайтеся, що ваші клієнти Microsoft Teams оновлено. Докладні відомості про оновлення клієнта див. в [статті Оновлення Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Якщо з якоїсь причини не вдається оновити клієнт, буде очищено більшість кешованих даних. Однак якщо проблеми не зникли після входу або виходу з системи, закрийте Teams і очистіть кеш клієнта, виконавши такі дії:
1. Закрийте Microsoft Teams.
2. Перейдіть до папки: %appdata%\microsoft\teams і видаліть усі файли.
3. Знову відкрити Microsoft Teams.
