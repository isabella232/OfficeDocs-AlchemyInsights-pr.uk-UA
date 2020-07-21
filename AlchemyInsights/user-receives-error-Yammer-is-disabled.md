---
title: Користувач отримує, помилка AADSTS7000112 Yammer вимкнуто
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198367"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Користувач отримує, помилка AADSTS7000112 Yammer вимкнуто

Якщо з'являється повідомлення про помилку "AADSTS7000112: застосунок" 00000005-0000-0ff1-ce00-000000000000 "(Yammer) вимкнуто", виникає проблема з принципалом служби в Azure AD. Можливо, адміністратор вимкнув принципал служби для блокування доступу до Yammer.

Вимкнення основної служби не рекомендується і може спричинити додаткові проблеми. Для отримання додаткових відомостей про підтримуваний підхід до блокування доступу користувачів до Yammer зверніться [до служби підтримки Yammer для користувачів Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Щоб вирішити цю проблему, на порталі Azure і відновлення доступу користувачів до Yammer:

1.  Відкрийте сторінку Azure Active Directory і виберіть **корпоративні програми** в області **керування** в лівій навігаційній панелі.
3.  Введіть **Office 365 Yammer** , у полі пошуку та виберіть ім'я програми, щоб відкрити параметри.
4.  Виберіть **Властивості** під **керування** в області переходів ліворуч.
5.  Встановити значення **увімкнуто для входу в систему?** щоб **так**, а потім виберіть **зберегти**.
6.  Увійдіть у Yammer знову. Можливо, потрібно буде очистити файли cookie.

Крім того, запустити команди PowerShell, щоб установити значення. Щоб отримати додаткові відомості, див ["Вибачте, але у нас виникли проблеми з входом" помилка під час натискання кнопки Yammer плитки в Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 