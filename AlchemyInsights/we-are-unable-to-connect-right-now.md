---
title: Проблеми з активацією – ми не можемо підключитися прямо зараз
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726004"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Виправлення програм Microsoft 365 "повідомлення зараз не вдається підключитися"

Якщо ви отримали це повідомлення, виконайте наведені нижче дії.

1. Перевірте брандмауер, антивірусне програмне забезпечення та параметри проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Microsoft 365. Переглянути [URL-адреси та діапазони IP-адрес Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Перейдіть на сторінку **Запуск**  >  **Run**, а потім введіть **Services. msc**. Переконайтеся, що всі наведені нижче служби запущено.
    - Параметри автоматичного настроювання підключених мережних пристроїв
    - Служба "список мереж"
    - Поінформованість про розташування мережі
    - Журнал подій Windows

Якщо один із цих служб не запущено, випробуйте її, щоб почати. Якщо у вас виникла проблема з запуском служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:

**SFC/SCANNOW**

Після завершення цієї команди перезавантажте комп'ютер.

Докладні відомості наведено в статті ["на жаль, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше під час активації Office із Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).