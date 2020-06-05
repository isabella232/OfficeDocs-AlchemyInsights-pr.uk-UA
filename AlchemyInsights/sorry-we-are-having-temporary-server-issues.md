---
title: Виправлення Microsoft 365 Apps Вибачте, у нас виникли тимчасові проблеми з сервером повідомлення
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582724"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Виправлення Microsoft 365 Apps "Вибачте, ми виникли проблеми з тимчасового сервера"

Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.

1. Перевірте настройки брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365. Перегляд [URL-адрес і діапазонів IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Перейдіть до **запуску**  >  **Run**, а потім введіть **Services. msc**. Переконайтеся, що виконуються такі служби:
    - Автоматичне настроювання мережних підключених пристроїв
    - Служба списку мереж
    - Поінформованість про розташування в мережі
    - Журнал подій Windows

Якщо одну з цих служб не запущено, спробуйте запустити його. Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:

**SFC/SCANNOW**

Після завершення цієї команди, перезавантажте комп'ютер.

Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).