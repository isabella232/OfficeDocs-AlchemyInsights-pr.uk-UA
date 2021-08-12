---
title: Read-Only обслуговування під час спроби використати SharePoint або OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910567"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only обслуговування під час спроби використати SharePoint або OneDrive

Під час спроби скористатися **програмою SharePoint** або OneDrive для одного з наведених нижче сценаріїв може з'явитися повідомлення "Обслуговування SharePoint доступне лише для читання. 

-   Запланована або активна дія обслуговування.  Щоб перевірити їх, перейдіть до [Центру повідомлень](https://portal.office.com/adminportal/home#/messagecenter).
-   З високим пріоритетом може виникнути інцидент активної служби. Перевірте наявність будь-яких порад або інцидентів, перейнявшись до [справності служби.](https://portal.office.com/adminportal/home#/servicehealth)
-   Незначний сценарій автоматичного відновлення, який може статися через неочікувані події на серверах, які можуть тривати менше 30 хв. тощо. 
    
    Для неповнолітніх відновлень немає дописів Центру повідомлень або Справності служби, але незабаром ви повернетесь до звичайних повідомлень.

У деяких випадках ми помічали, що з'явилося одна з трьох наведених вище сценаріїв, і службу відновлено, але кеш браузера користувачів не очищено.

Перш ніж переходити на сайт, спробуйте очистити кеш браузера.

1. У браузері Microsoft Edge виберіть елементи **Настройки**, а потім – **Конфіденційність і безпека**.
2. У **розділі Очистити перегляд** виберіть елемент **Виберіть, що потрібно очистити.**
3. Виберіть **файли cookie та збережені дані веб-сайтів**, а потім натисніть кнопку **Очистити**.

>[!Note] 
> Ці дії можуть відрізнятися, якщо використовується інші браузери, як-от Mozilla Firefox або Google Chrome.

>[!Note] 
> Інший варіант – відкрити сайт або SharePoint в OneDrive у новому вікні InPrivate.