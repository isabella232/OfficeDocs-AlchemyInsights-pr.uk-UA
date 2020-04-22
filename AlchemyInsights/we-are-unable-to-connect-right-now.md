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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716193"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Виправлення програми Office "не вдається підключитися зараз" повідомлення

Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.

1. Перевірте брандмауер, антивірусне програмне забезпечення та настройки проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Office. Переглянути [URL-адреси Microsoft і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Перейдіть до **запуску** > **, а**потім введіть **Services. msc**. Переконайтеся, що виконуються такі служби:
    - Автоматичне настроювання мережних підключених пристроїв
    - Служба списку мереж
    - Поінформованість про розташування в мережі
    - Журнал подій Windows

Якщо одну з цих служб не запущено, спробуйте запустити його. Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:

**SFC/SCANNOW**

Після завершення цієї команди, перезавантажте комп'ютер.

Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації Office з Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).