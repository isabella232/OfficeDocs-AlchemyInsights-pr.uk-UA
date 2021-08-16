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
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998193"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Виправлення помилок програм Microsoft 365 "Не вдалося підключитися зараз"

Якщо ви отримали це повідомлення, спробуйте виконати такі дії:

1. Перевірте параметри брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету Microsoft 365 програм. Докладні [відомості див. в статті Діапазони URL- і IP-адрес Корпорації Майкрософт.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Відкрийте меню **"Пуск"**  >  і введіть **services.msc.** Переконайтеся, що всі ці служби запущено:
    - Автоматичне настроювання підключених мережевих пристроїв
    - Служба списку мережі
    - Усвідомлення мережевого розташування
    - Windows Журнал подій

Якщо одну з цих служб не запущено, спробуйте запустити її. Якщо під час запуску служби відобразиться помилка, запустіть наведену нижче команду, відкривши командний рядок із дозволами в режимі адміністратора.

**sfc /scannow**

Коли ця команда завершиться, перезавантажте комп'ютер.

Докладні відомості див. в [розділі "На жаль, не вдалося підключитися до вашого облікового запису. Спробуйте ще раз пізніше" під час активації Office з Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).