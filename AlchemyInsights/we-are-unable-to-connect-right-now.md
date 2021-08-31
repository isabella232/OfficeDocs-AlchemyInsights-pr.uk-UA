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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744616"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Виправлення помилок із Microsoft 365 "Не вдалося підключитися"

Примітка. Якщо ви використовуєте попередню версію Windows (наприклад, Windows 7 із пакетом оновлень 1 (SP1), Windows [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Server 2008 R2), скористайтеся засобом простого виправлення, щоб увімкнути TLS 1.2 за замовчуванням. Докладні відомості див. в статтях Оновлення для ввімкнення [протоколів TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)як безпечних протоколів за замовчуванням у WindowsHTTP у Windows.

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