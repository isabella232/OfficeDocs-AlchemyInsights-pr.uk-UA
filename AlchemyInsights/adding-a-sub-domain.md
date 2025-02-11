---
title: Додавання дочірніх доменів
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506766"
---
# <a name="adding-a-sub-domain"></a>Додавання дочірніх доменів

Дочірні домени можна додавати до того самого або іншого клієнта, ніж батьківський домен. У будь-якому разі ви повинні самостійно керувати параметрами DNS на веб-сайті реєстратора. Якщо ви дозволили корпорації Майкрософт керувати параметрами DNS із записами DNS-серверів або придбали домен у корпорації Майкрософт, ви не зможете додати дочірні домени, не змінюючи цей домен.

Спочатку додайте батьківський домен, а потім додайте дочірні домени. Якщо дочірнімдоменом є один і той самий клієнта, додаткової перевірки не потрібно. Якщо додати до окремого клієнта дочірні домени, для перевірки права власності на домен потрібен запис TXT DNS, перш ніж додавати домен і додаткові записи DNS для вибраних служб.

- Щоб додати домен або дочірні домени, виконайте вказівки майстра додавання домену [або](https://admin.microsoft.com/Adminportal#/Domains/Wizard)додайте домен чи дочірні домени вручну, перейшоввши до пункту Настроювання   >  **домену**  >  **Додати домен**.

За потреби:

- Щоб змінити список користувачів, які керують параметрами DNS для наявного домену, на вкладці **Настройки**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home#/Domains)(Домени) , установіть прапорець поруч із доменом, а потім виберіть елемент Manage DNS (Керування службою **DNS).** У майстрі виберіть **пункт Додати власні записи DNS** і виконайте роботу майстра.
- Щоб додати дочірні домени до придбаного домену Microsoft, спочатку перенесіть домен до іншого реєстратора, а потім внесіть наведені вище зміни, щоб керувати власними записами DNS. Інструкції див. в [статті Перенесення домену з корпорації Майкрософт до іншого хоста.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Якщо ви отримали повідомлення про помилку, що ваш домен уже використовується іншими учасниками або користувачами у вашій організації, спочатку потрібно взяти на себе цей некерований обліковий запис, перш ніж використовувати домен. Указівки наведено в статті Керування некерованою [каталогом](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)у Azure Active Directory .
