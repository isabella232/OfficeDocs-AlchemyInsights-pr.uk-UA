---
title: Проблема з активацією – не вдалося підключитися зараз
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806463"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Виправлення помилок у програмах Microsoft 365 "Не вдалося підключитися зараз"

Якщо ви отримали це повідомлення, спробуйте виконати такі дії:

1. Перевірте параметри брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365. Докладні [відомості див. в статті Діапазони URL- і IP-адрес Корпорації Майкрософт.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Відкрийте меню **"Пуск"**  >  і введіть **services.msc.** Переконайтеся, що всі ці служби запущено:
    - Автоматичне настроювання підключених мережевих пристроїв
    - Служба списку мережі
    - Усвідомлення мережевого розташування
    - Журнал подій Windows

Якщо одну з цих служб не запущено, спробуйте запустити її. Якщо під час запуску служби відобразиться помилка, запустіть наведену нижче команду, відкривши командний рядок із дозволами в режимі адміністратора.

**sfc /scannow**

Коли ця команда завершиться, перезавантажте комп'ютер.

Докладні відомості див. в [розділі "На жаль, не вдалося підключитися до вашого облікового запису. Спробуйте ще раз пізніше" під час активації Office зі служби Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)