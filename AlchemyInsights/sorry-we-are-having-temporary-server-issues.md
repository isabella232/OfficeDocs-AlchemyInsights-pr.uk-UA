---
title: Повідомлення Microsoft 365 про тимчасові проблеми із сервером в програмах, на жаль, виникають тимчасові проблеми із сервером
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
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021617"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Виправлення неполадок із Microsoft 365 "На жаль, у нас виникли тимчасові проблеми із сервером"

Якщо ви отримали це повідомлення, спробуйте виконати такі дії:

1. Перевірте параметри брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету Microsoft 365 програм. Див. [номери URL-адрес і діапазони IP-адрес.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Відкрийте меню **"Пуск"**  >  і введіть **services.msc.** Переконайтеся, що всі ці служби запущено:
    - Автоматичне настроювання підключених мережевих пристроїв
    - Служба списку мережі
    - Усвідомлення мережевого розташування
    - Windows Журнал подій

Якщо одну з цих служб не запущено, спробуйте запустити її. Якщо під час запуску служби відобразиться помилка, запустіть наведену нижче команду, відкривши командний рядок із дозволами в режимі адміністратора.

**sfc /scannow**

Коли ця команда завершиться, перезавантажте комп'ютер.

Докладні відомості див. в [розділі "На жаль, не вдалося підключитися до вашого облікового запису. Спробуйте ще раз пізніше" під час активації](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).