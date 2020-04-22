---
title: 1065 вилучення ПЕРІОДУ, вихідний IP-адреса rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704618"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Вилучення діапазону вихідних IP-адрес на кінець періоду

Ми виявили потенційні проблеми з організацією, яка (якщо не виправити 26 жовтня, 2018) може розірвати потік пошти до локальної або зовнішньої призначення. Як раніше повідомляється, для спрощення керування IP-адрес, ми консолідація Exchange Online захист (кінець періоду) IP-адреса діапазони, які використовуються для надсилання й отримання електронної пошти за межами Microsoft 365. Наш аналіз вказує на те, що один або кілька зовнішніх джерел електронної пошти або місця призначення, які ви настроїли з'єднувачі для потоку пошти, не приймає підключення з IP-адресу діапазонів показано [тут](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Закон до 26 жовтня для забезпечення цих джерел і напрямків буде приймати підключення до і з усіх [опублікованих кінець періоду IP-адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Щоб отримати додаткові відомості про цю зміну, будь ласка, перегляньте повідомлення центру повідомлень [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Примітка**: Якщо ви раніше використовували IP або URL публікації через HTML, XML і RSS для оновлення кінцевої точки, ви також повинні перейти на нові веб-сервіси для автоматизації цих типів оновлень. Щоб отримати додаткові відомості див. [корпорація майкрософт 365 кінцевої точки категорій та Microsoft 365 IP-адресу та URL веб-служби](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
