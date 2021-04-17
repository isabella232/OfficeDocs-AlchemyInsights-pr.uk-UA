---
title: Вирішення проблем із програмами Microsoft 365Повідомлення про тимчасові проблеми із сервером
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835292"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Виправлення помилок у програмах Microsoft 365 "На жаль, виникають тимчасові проблеми із сервером"

Якщо ви отримали це повідомлення, спробуйте виконати такі дії:

1. Перевірте параметри брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365. Див. [номери URL-адрес і діапазони IP-адрес.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Відкрийте меню **"Пуск"**  >  і введіть **services.msc.** Переконайтеся, що всі ці служби запущено:
    - Автоматичне настроювання підключених мережевих пристроїв
    - Служба списку мережі
    - Усвідомлення мережевого розташування
    - Журнал подій Windows

Якщо одну з цих служб не запущено, спробуйте запустити її. Якщо під час запуску служби відобразиться помилка, запустіть наведену нижче команду, відкривши командний рядок із дозволами в режимі адміністратора.

**sfc /scannow**

Коли ця команда завершиться, перезавантажте комп'ютер.

Докладні відомості див. в [розділі "На жаль, не вдалося підключитися до вашого облікового запису. Спробуйте ще раз пізніше" під час активації](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).