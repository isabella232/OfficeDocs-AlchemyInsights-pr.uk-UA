---
title: Активація питання-ми не вдалося підключитися зараз
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581896"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Виправлення Microsoft 365 програм "ми не вдається підключитися зараз" повідомлення

Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.

1. Перевірте настройки брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365. Переглянути [URL-адреси Microsoft і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Перейдіть до **запуску**  >  **Run**, а потім введіть **Services. msc**. Переконайтеся, що виконуються такі служби:
    - Автоматичне настроювання мережних підключених пристроїв
    - Служба списку мереж
    - Поінформованість про розташування в мережі
    - Журнал подій Windows

Якщо одну з цих служб не запущено, спробуйте запустити його. Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:

**SFC/SCANNOW**

Після завершення цієї команди, перезавантажте комп'ютер.

Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації Office з Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).