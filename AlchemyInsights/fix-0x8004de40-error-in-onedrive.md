---
title: Виправлення 0x8004de40 oneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649769"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Виправлення 0x8004de40 oneDrive

Якщо під час роботи з Windows 7 з'являється таке повідомлення про помилку, оновіть windows, щоб активувати [протоколИ TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)як безпечні протоколи за замовчуванням у WindowsHTTP.

Якщо використовується Windows 10 і з'являється повідомлення про помилку 0x8004de40 OneDrive:

- Перезавантажте комп'ютер, на який це вплине, підключившись до домену Acitve Directory.
- Якщо перезавантаження не допомогло вирішити проблему, повторно під'єдайте свій пристрій з Azure AD. 

**Примітка.** Ці кроки потрібно розташувати в корпоративній мережі. Не виконуйте ці дії, коли не підключено до корпоративної інфраструктури (наприклад, під час подорожі). 

1. Відкрийте командний рядок у режимі адміністратора, натиснувши **кнопку** Пуск , клацніть правою кнопкою **миші** пункт Командний рядок і виберіть **команду Запустити із правами адміністратора**.

1. Введіть *dsregcmd /leave і* натисніть клавішу **Enter.**

1. Після завершення введіть *dsregcmd /join і* натисніть **клавішу Enter.**

1. Коли завершите, закрийте командний рядок.

1. Перезавантажте комп'ютер і ввійдіть у OneDrive.