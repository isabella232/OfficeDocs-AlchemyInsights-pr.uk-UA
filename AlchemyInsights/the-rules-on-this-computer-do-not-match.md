---
title: Помилка. Правила на цьому комп'ютері не збігаються
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981134"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Помилка. Правила на цьому комп'ютері не збігаються

Відомості про те, як переглянути оновлений стан відомої проблеми, див. в статті Правила на цьому [комп'ютері](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) не відповідають правилам microsoft Exchange

Команда Outlook в збірці 12928.10000. Виправлення вже доступне в програмі оцінювачів із ралі та перейде до щомісячного каналу оновлення наприкінці червня 2020 р. Коли ви вкажете фіксовану збірку, може з'явитися повідомлення "Які правила слід зберігати" один раз востаннє. Коли з'явиться відповідний запит, виберіть Сервер, а потім поверніться Outlook знову ввімкніть усі вимкнуті правила.

Доки виправлення не з'явиться, скористайтеся наведеним нижче способом вирішення.

**Спосіб вирішення. У** нещодавніх звітах ця проблема виникла лише для тих, хто створив правила клієнта лише Outlook настільному комп'ютері. Якщо проблема не зникне, рекомендовано видалити їх, а потім створити й відредагувати правила лише в OWA (Outlook Web App), доки проблему не буде вирішено.

Якщо видалити правила вручну не можна, Outlook команди під час запуску Outlook запустивши Outlook.exe /cleanrules. При цьому буде видалено правила клієнта та сервера. Усі правила для всіх облікових записів у профілі Outlook видаляться. Цю команду додатково описано в статті Перемикачі командного рядка.

