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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329469"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only обслуговування під час спроби використати SharePoint або OneDrive

Користувачі можуть отримати повідомлення **"Обслуговування"** лише для читання під час спроби скористатися SharePoint або OneDrive для одного з наведених нижче сценаріїв. 

-   Запланована або активна дія обслуговування.  Щоб перевірити їх, перейдіть до [Центру повідомлень](https://portal.office.com/adminportal/home#/messagecenter).
-   З високим пріоритетом може виникнути інцидент активної служби. Перевірте наявність будь-яких порад або інцидентів, перейвши до [справності служби.](https://portal.office.com/adminportal/home#/servicehealth)
-   Незначний сценарій автоматичного відновлення, який може статися через неочікувані події на серверах, які можуть тривати менше 30 хв. тощо. 
    
    Для неповнолітніх відновлень немає дописів Центру повідомлень або Справності служби, але незабаром ви повернетесь до звичайних повідомлень.

У деяких випадках ми помічали, що з'явилося одна з трьох наведених вище сценаріїв, і службу відновлено, але кеш браузера користувачів не очищено.

Перш ніж переходити на сайт, спробуйте очистити кеш браузера.

1. У браузері Microsoft Edge виберіть **Настройки**, а потім – **Конфіденційність і безпека**.
2. У **розділі Очистити перегляд** виберіть елемент **Виберіть, що потрібно очистити.**
3. Виберіть **файли cookie та збережені дані веб-сайтів**, а потім натисніть кнопку **Очистити**.

**Примітка.** Ці дії можуть відрізнятися, якщо використовується інші браузери, як-от Mozilla Firefox або Google Chrome.

**Примітка.** Інший варіант – відкрити свій SharePoint або відкрити OneDrive в новому вікні InPrivate.