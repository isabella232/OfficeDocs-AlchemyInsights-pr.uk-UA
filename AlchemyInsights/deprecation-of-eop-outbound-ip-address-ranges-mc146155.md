---
title: 1065 про несхвалення EOP вихідної IP-адреси rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806816"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Несхвалення вихідних діапазонів IP-адрес EOP

Ми виявили потенційну проблему з організацією, яка (якщо не виправлено від 26 жовтня 2018), може призвести до розриву потоку пошти до локальних або зовнішніх напрямків. Як повідомлялося раніше, щоб спростити керування діапазоном IP-адрес, ми Зміцнімо діапазони IP-адрес захисту Exchange Online (EOP), які використовуються для надсилання й отримання електронної пошти за межі Microsoft 365. Наш аналіз вказує на те, що один або кілька із зовнішніх джерел електронної пошти або пунктів призначення, настроєні в з'єднаннях пошти, не приймають з'єднання з діапазонів IP-адрес, що відображаються [тут](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Дії перед 26 жовтня для забезпечення цих джерел і призначень буде приймати підключення до та від всіх [опублікованих IP-адрес EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Щоб отримати докладні відомості про ці зміни, ознайомтеся з відомостями про повідомлення центру повідомлень [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Примітка**. Якщо ви раніше використовували IP-адресу або публікацію URL-адрес за допомогою HTML, XML і RSS для оновлень кінцевої точки, ви також повинні перейти до нових веб-служб для автоматизації цих типів оновлень. Щоб отримати докладніші відомості, ознайомтеся з [категоріями кінцевих точок microsoft 365 і microsoft 365 IP-адресою та веб-службою URL-адресою](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
