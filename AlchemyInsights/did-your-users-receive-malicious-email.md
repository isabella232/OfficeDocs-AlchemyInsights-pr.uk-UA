---
title: Чи ваші користувачі отримували зловмисні електронні листи
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326731"
---
# <a name="did-your-users-receive-malicious-email"></a>Чи ваші користувачі отримували зловмисні електронні листи?

Тепер ви можете повідомити корпорації Майкрософт про зловмисні електронні листи за допомогою надсилання [Microsoft 365 Defender порталі](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Повідомлення, надіслані [](https://security.microsoft.com/reportsubmission?viewid=admin) в надіслані адміністратором надіслані адміністратором, скануються, а в розгорнутому меню докладно показано такі результати:

- Чи сталася помилка автентифікації електронного листа відправника під час доставки.
- Інформація про збіги з політиками, які могли вплинути на вердикт для повідомлення або перевизначити його.
- Поточні результати знешкодження, які дають змогу побачити, чи URL-адреси або файли, які містить повідомлення, були зловмисними, чи ні.
- Відгуки оцінювачів

Якщо знайдено перевизначення, потрібно провести повторне сканування через кілька хвилин. Якщо не виникало проблем з автентифікацією електронного листа і перевизначення не вплинуло на доставку, обробка відгуків оцінювачів може зайняти до одного дня.

Якщо ви не згідні з остаточним вердиктом для повідомлення, URL-адреси або файлу (заблоковано чи не заблоковано), надішліть повідомлення знову для повторного сканування через день. Вірогідність того, що вердикт зміниться після повторного надсилання повідомлення, висока.

Тим часом, зловмисні електронні листи можна вилучити з поштових скриньок користувачів, дотримуючись вказівок із [цієї статті](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Клієнти, у яких є Microsoft Defender для Office 365, можуть:
  - Пошук [і видалення підозрілих](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered) електронних листів за допомогою провідника загроз
  - [Використання Сейф посилань для блокування доступу](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) до зловмисної URL-адреси
  - Відстеження користувачів, які клацали зловмисні URL-адреси та отримували до них доступ: перегляд [фішингнових URL-адрес](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)і клацання verdict data  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Запуск [автоматичного дослідження вручну](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Ви також можете захистити себе від зловмисних файлів і URL-адрес, дотримуючись вказівок зі статті [Захист від зловмисних URL-адрес і файлів](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
