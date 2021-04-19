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
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815267"
---
# <a name="did-your-users-receive-malicious-email"></a>Чи ваші користувачі отримували зловмисні електронні листи?

- Тепер ви можете повідомити корпорації Майкрософт про зловмисні електронні листи за допомогою [надходжень від адміністратора в Центрі безпеки та відповідності](https://sip.protection.office.com/reportsubmission).

Повідомлення, надіслані до [надходжень від адміністратора](https://sip.protection.office.com/reportsubmission), скануються, і в спливаючому меню **відомостей** відображаються такі результати:

- Чи сталася помилка автентифікації електронного листа відправника під час доставки.
- Інформація про збіги з політиками, які могли вплинути на вердикт для повідомлення або перевизначити його.
- Поточні результати знешкодження, які дають змогу побачити, чи URL-адреси або файли, які містить повідомлення, були зловмисними, чи ні.
- Відгуки оцінювачів

Якщо знайдено перевизначення, потрібно провести повторне сканування через кілька хвилин. Якщо не виникало проблем з автентифікацією електронного листа і перевизначення не вплинуло на доставку, обробка відгуків оцінювачів може зайняти до одного дня.

Якщо ви не згідні з остаточним вердиктом для повідомлення, URL-адреси або файлу (заблоковано чи не заблоковано), надішліть повідомлення знову для повторного сканування через день. Вірогідність того, що вердикт зміниться після повторного надсилання повідомлення, висока.

Тим часом, зловмисні електронні листи можна вилучити з поштових скриньок користувачів, дотримуючись вказівок із [цієї статті](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Клієнти, у яких є Microsoft Defender для Office 365, можуть:
    - використовувати [Викривальник загроз для пошуку та видалення підозрілих електронних листів](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered);
    - [використовувати Безпеку посилань для блокування доступу](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) до зловмисних URL-адрес;
    - відстежувати користувачів, які клацнули зловмисні URL-адреси й отримали доступ до них: [Перегляд URL-адрес фішингу та клацання даних вердикту](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace);
    - уручну [запустити автоматичну перевірку](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).

Ви також можете захистити себе від зловмисних файлів і URL-адрес, дотримуючись вказівок зі статті [Захист від зловмисних URL-адрес і файлів](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).