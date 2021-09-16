---
title: У звітах у Центрі адміністрування Microsoft 365 не відображаються читабельні імена користувачів
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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327835"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>У звітах у Центрі адміністрування Microsoft 365 не відображаються читабельні імена користувачів

У звітах у Центрі адміністрування Microsoft 365 відображаються не імена користувачів, а буквено-числові значення, наприклад B2BC6C15BB9FCDEA71E5CD302D228CC8.

Це очікувана поведінка, яка повідомляється в Центр повідомлень (MC275344, опубліковано 3 серпня 2021 р.). 

Глобальні адміністратори можуть скасувати цю зміну для свого осередку та відобразити ідентифікаційні дані користувача, якщо це дозволено правилами організації щодо приватності. Щоб скасувати зміну для осередку:

1. У Центрі адміністрування відкрийте **Параметри**  >  **Параметри організації**  >  [**Служби**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) та виберіть **Звіти**. 
1. У розділі **Виберіть спосіб відображення відомостей про користувача** виберіть параметр **Відображати ідентифікаційні дані користувачів у звітах**, а потім повторно запустіть звіт.