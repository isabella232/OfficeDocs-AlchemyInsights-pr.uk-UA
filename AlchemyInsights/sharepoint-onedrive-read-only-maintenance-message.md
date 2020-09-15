---
title: Під час спроби використовувати службу SharePoint або OneDrive можна тільки для читання.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670853"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Під час спроби використовувати службу SharePoint або OneDrive можна тільки для читання.

Користувачі можуть отримувати повідомлення **лише для читання** , коли ви намагаєтеся використовувати SharePoint або OneDrive для одного з наведених нижче сценаріїв. 

-   Заплановані або активні дії з обслуговування.  Перевірте їх, перейшовши до [центру повідомлень](https://portal.office.com/adminportal/home#/messagecenter).
-   Високий пріоритет, активна служба, що може бути відбувається. Перегляньте всі рекомендації та інциденти, перейшовши до [справності служби](https://portal.office.com/adminportal/home#/servicehealth).
-   Незначний сценарій відновлення для автоматичного зцілення, який може відбуватися через непередбачені події на серверах, які можуть тривати менше 30 хв. 
    
    Для цих незначних відшкодувань немає повідомлень або служб для медичних повідомлень, але ви маєте повернутися до нормального.

У дуже мало випадків ми спостерігали, що один із трьох сценаріїв, перерахованих вище, було причиною, а служба відновлено, але кеш браузера користувачів не очищено.

Перш ніж переходити до сайту, спробуйте очистити кеш браузера.

1. У браузері Microsoft EDGE натисніть кнопку **настройки**, а потім виберіть пункт **конфіденційність і безпека**.
2. У розділі **Очистити перегляд**виберіть пункт **вибрати, що потрібно очистити**.
3. Виберіть **файли cookie та збережені дані веб-сайту**, а потім натисніть кнопку **Очистити**.

>[!Note] 
> Ці дії можуть відрізнятися під час використання інших браузерів, таких як Mozilla Firefox або Google Chrome.

>[!Note] 
> Інший варіант – відкрити сайт SharePoint або OneDrive в новому вікні InPrivate.