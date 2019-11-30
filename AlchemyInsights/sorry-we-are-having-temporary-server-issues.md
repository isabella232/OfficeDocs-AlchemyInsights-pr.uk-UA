---
title: Виправлення програм Office Вибачте, у нас виникли тимчасові проблеми з сервером повідомлення
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628011"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Фіксація програм Office "Вибачте, у нас виникли проблеми з тимчасовим сервером"

Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.

1. Перевірте брандмауер, антивірусне програмне забезпечення та настройки проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Office. Перегляньте [URL-адреси Office 365 і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Перейдіть до **запуску** > **, а**потім введіть **Services. msc**. Переконайтеся, що виконуються такі служби:
    - Автоматичне настроювання мережних підключених пристроїв
    - Служба списку мереж
    - Поінформованість про розташування в мережі
    - Журнал подій Windows

Якщо одну з цих служб не запущено, спробуйте запустити його. Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:

**SFC/SCANNOW**

Після завершення цієї команди, перезавантажте комп'ютер.

Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації Office з Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).