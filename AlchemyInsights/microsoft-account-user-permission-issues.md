---
title: Виправлення неполадок із проблемою – користувач не знайдено в каталозі
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725428"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Виправлення неполадок із проблемою – користувач не знайдено в каталозі

Якщо користувачі отримують повідомлення про помилку "користувач не може знайти" в каталозі, спробуйте ще раз, коли тип проблеми – користувач, який не належить до каталогу.

Щоб вирішити цю проблему, можна виконати наведені нижче дії.

- Переконайтеся, що обліковий запис, який прийняв запрошення на повідомлення електронної пошти, – це той самий обліковий запис, який використовується для входу в пізнішу версію. Переконайтеся, що користувач використовує той самий обліковий запис, щоб прийняти запрошення та ввійти на сайт. 

Щоб отримати докладні відомості, Дізнайтеся, [як керувати псевдонімами для облікового запису Microsoft, </a> щоб керувати входом до служби Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Перейдіть до кожного веб-сайту, у якому користувач отримує повідомлення про помилку. 

Add ("/_layouts/15/Peopl.aspx/membershippid = 0" (у межах двох лапок) до кінця URL-адреси сайту. 

Приклад: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Виберіть користувача зі списку.

- Натисніть кнопку **Видалити дозволи користувача** на стрічці. 
-  Додайте назад користувача та надішліть запрошення до користувача.

