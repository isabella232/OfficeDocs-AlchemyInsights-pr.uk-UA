---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 7bb5ec0efb7e29dc6a133d62491c7674c5a851a4fa422c647035aeaa0dbcd8d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918380"
---
# <a name="alert-policies"></a>Політики оповіщень

Центр безпеки Microsoft 365 безпеки & містить стандартні політики оповіщень, які ініціують оповіщення для організацій із передплатою на план "Office 365 для підприємств або Office 365 для державних установ США (E1, G1, E3, G3) або E5/G5. [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) Таким чином, адміністратори можуть отримати оповіщення електронною поштою, надіслане Office365Alerts@microsoft.com з рядком теми, наприклад "A low-severity alert: *name of alert policy"*(Оповіщення з низькою важливістю: назва політики оповіщення). Оповіщення надсилаються, коли для поширених дій надсилаються оповіщення, наприклад коли користувачі:

- Створіть правила для папки "Вхідні", які пересилатимуться електронні листи.
- Призначте дозволи своїй поштовій скриньці.
- Надається спільний доступ до великої кількості файлів і видаляйте їх SharePoint спільному доступу до них.
- Створювати пошукові запити для витребування електронної пошти та експортувати результати пошуку.

Щоб переглянути оповіщення та діяти над оминете його,

1. Перейдіть до Центру [безпеки & відповідності та](https://protection.office.com) ввійдіть у неї.
2. Натисніть **кнопку Оповіщення**  >  **Переглянути оповіщення.**
3. Клацніть оповіщення, щоб відобразити сплітаючу сторінку з відомостями про оповіщення.

До оповіщення можна виконати певні дії, наприклад видалити підозрілі правила для папки ["Вхідні"](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Крім того, ви можете просто закрити оповіщення, натиснувши **кнопку** Вирішити на сповіщень.

Докладні відомості про настроювання політик оповіщень і керування ами див. в [цій статті.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Увага!** Оповіщення про сповіщення електронною поштою від корпорації Майкрософт ніколи не питатиме вас про такі дії:

- Введення пароля
- Перевірка відомостей про безпеку облікового запису
- Повторна автентифікація

Якщо ви отримали таке повідомлення електронної пошти, корпорація Майкрософт не надіслала його й вважається фішингом. У такому разі повідомте [про це в корпорації Майкрософт.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)