---
title: Журнали паролів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527775"
---
# <a name="password-logs"></a>Журнали паролів

**Проблеми з доступом до журналів аудиту скидання пароля**

Щоб вирішити проблеми, пов'язані з доступом до журналів аудиту для скидання пароля, виконайте наведені нижче дії.

Переконайтеся, що ви маєте право переглядати журнали аудиту. 

Авторизовані лише такі ролі:
 - Глобальний адміністратор
 - Адміністратор системи безпеки
 - Читач безпеки

**Я хочу Переглянути всі події перевірки скидання пароля з моменту, коли ви спочатку розгорнули**

За останні 30 днів у звітах про зміни пароля та реєстраційних подій 120 000 зберігаються. Цей максимальний ліміт застосовується до інтерфейсу користувача під час завантаження файлу CSV. події 1 000 000 доступні за допомогою PowerShell.
Щоб отримати докладніші відомості, ознайомтеся з наведеними нижче посиланнями.

- [Повідомлення про те, що для самостійного скидання пароля з неавтоматичної служби й API подій](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Швидке завантаження подій для реєстрації паролів швидко за допомогою PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Я хочу дізнатися більше про можливості звітування про скидання пароля**

Перевірка користувачів, які реєструють або скиньте паролі за допомогою журналів аудиту Azure AD для скидання пароля на порталі "Лазурний" в розділі " **користувачі та групи**".
Щоб отримати докладніші відомості, ознайомтеся з такими посиланнями:

- [Огляд звітів про скидання пароля](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Перегляд звітів про скидання пароля на порталі «Лазурний»](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Повідомлення про те, що для самостійного скидання пароля з неавтоматичної служби й API подій](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Швидке завантаження подій для реєстрації паролів швидко за допомогою PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


