---
title: 1065 несхвалення EOP Вихідна IP-адреса rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404842"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Несхвалення EOP вихідне Вихідна IP-адреса

Це свідчить потенційна проблема з вашої організації, які (якщо не виправити, 26 жовтня 2018) може порушити потік пошти локальні або зовнішні джерела. Як раніше передано спростити IP адреса діапазон керування, ми ти консолідації діапазони Exchange Online захисту (EOP) IP-адрес, які використовуються для надсилання й отримання електронної пошти за межами Office 365. Наш аналіз показує, що подані зовнішню поштову джерела або місця, які ви налаштували у роз'ємах потік пошти не приймає підключення з на IP адреса діапазони показано [тут](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Виступати перед 26 жовтня для забезпечення цих джерел та напрямків буде приймати з'єднання і від всіх [опубліковані EOP IP-адрес](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Щоб отримати додаткові відомості про цю зміну будь ласка, дивіться центрі повідомлень повідомлення з [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Примітка**: Якщо ви раніше використовували IP або URL публікації за допомогою HTML, XML та RSS для кінцевої точки оновлень, також повинні міграцією до нових веб-сервісів для автоматизації ці типи оновлень. Докладніше перегляньте [Office 365 кінцевої точки категорії та Office 365 IP-адреси та URL-адресу веб-служби](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
