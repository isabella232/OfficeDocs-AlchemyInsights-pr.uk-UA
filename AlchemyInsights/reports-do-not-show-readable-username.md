---
title: Звіти в Центр адміністрування Microsoft 365 ім'я користувача, який не можна прочитати
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316355"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Звіти в Центр адміністрування Microsoft 365 ім'я користувача, який не можна прочитати

У звітах Центр адміністрування Microsoft 365 не відображатимуться імена користувачів, а алфавітні числові значення, наприклад B2BC6C15BB9FCDEA71E5CD302D228CC8.

Це очікувана поведінка, яка повідомляється в Центрі повідомлень (MC275344, опублікованій 3 серпня 2021 р.). 

Глобальні адміністратори можуть повернутися до цієї зміни для свого клієнта та відобразити особисті відомості про користувача, якщо це дозволено в організації. Щоб повернутися до змін клієнта:

1. У Центрі адміністрування перейдіть до меню **Настройки**  >  **параметри оцінюєте**  >  [**служби**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)та виберіть **Звіти**. 
1. У **розділі Виберіть спосіб відображення відомостей про** користувача виберіть **параметр** Відображати особисті відомості у звітах, а потім повторно запустіть звіт.