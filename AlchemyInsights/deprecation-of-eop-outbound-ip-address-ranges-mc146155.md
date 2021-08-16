---
title: 1065 Вилучення діапазонів вихідних IP-адрес EOPMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031283"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Вилучення діапазонів вихідних IP-адрес EOP

Ми виявили потенційну проблему з вашою організацією, яка може порушити потік пошти до локальних або зовнішніх місць призначення (якщо не виправлено до 26 жовтня 2018 р.). Як повідомлялось раніше, щоб спростити керування діапазоном IP-адрес, ми об'єднуємо діапазони IP-адрес Exchange Online Protection (EOP), які використовуються для надсилання й отримання електронної пошти за межами Microsoft 365. Наш аналіз указує на те, що одне або кілька зовнішніх джерел електронної пошти або місць призначення, налаштовані в з'єднаторах потоків пошти, не приймають підключення з діапазонів IP-адрес, які відображаються [тут.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Виконайте дії до 26 жовтня, щоб переконатися, що ці джерела та місця призначення прийматимуться підключення до всіх опублікованих [IP-адрес EOP і](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)з них.

Докладні відомості про цю зміну див. в публікаціях у Центрі повідомлень [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Примітка.** Якщо ви раніше використовували публікацію IP-адрес або URL-адрес за допомогою оновлень служб HTML, XML і RSS для оновлень кінцевих точок, потрібно також перенести до нових веб-служб, щоб автоматизувати ці типи оновлень. Докладні відомості див. в Microsoft 365 категорії [кінцевих точок і Microsoft 365 IP-адреси та веб-службу URL-адрес.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
