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
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312708"
---
# <a name="alert-policies"></a>Політики оповіщень

Microsoft 365 містить політики [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) оповіщень за замовчуванням, які ініціюють оповіщення для організацій із передплатою Microsoft 365 для підприємств або Microsoft 365 урядових організацій США (E1, G1, E3, G3 або E5/G5). Таким чином, адміністратори можуть отримати оповіщення електронною поштою, надіслане Office365Alerts@microsoft.com з рядком теми, наприклад "A low-severity alert: *name of alert policy"*(Оповіщення з низькою важливістю: назва політики оповіщення). Оповіщення надсилаються, коли для поширених дій надсилаються оповіщення, наприклад коли користувачі:

- Створіть правила для папки "Вхідні", які пересилатимуться електронні листи.
- Призначте дозволи своїй поштовій скриньці.
- Надається спільний доступ до великої кількості файлів або видаляється з них, SharePoint спільний доступ до файлів.
- Створювати пошукові запити для витребування електронної пошти та експортувати результати пошуку.

Щоб переглянути оповіщення та діяти над оминете його,

1. Виконайте одну з таких дій:
   - У меню Центр відповідності Microsoft 365 <https://compliance.microsoft.com> виберіть **оповіщення.** Або, щоб перейти безпосередньо на сторінку **"Оповіщення",** скористайтеся <https://compliance.microsoft.com/compliancealerts> .
   - На порталі Microsoft 365 Defender перейдіть до меню Інциденти, & <https://security.microsoft.com>  \> **оповіщення.** Або, щоб перейти безпосередньо на сторінку **"Оповіщення",** скористайтеся <https://security.microsoft.com/alerts> .
2. Клацніть оповіщення, щоб відобразити сплітаючу сторінку з відомостями про оповіщення.

До оповіщення можна виконати певні дії, наприклад видалити підозрілі правила для папки ["Вхідні"](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Крім того, ви можете просто закрити оповіщення, натиснувши кнопку **Усунути** на спліт-сторінці оповіщення.

Докладні відомості про настроювання політик оповіщень і керування ами див. в [цій статті.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Увага!** Оповіщення про сповіщення електронною поштою від корпорації Майкрософт ніколи не питатиме вас про такі дії:

- Введення пароля
- Перевірка відомостей про безпеку облікового запису
- Повторна автентифікація

Якщо ви отримали повідомлення електронної пошти з такими типами запитів, корпорація Майкрософт не надіслала його та вважається фішингом. Якщо ви отримаєте повідомлення з такими типами запитів, повідомте [про це корпорації Майкрософт.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)
