---
title: Усунення несправностей – користувач не знайдено в каталозі
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098191"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Усунення несправностей – користувач не знайдено в каталозі

Якщо користувачі отримують повідомлення про помилку "Не вдалося знайти користувача" в каталозі, спробуйте ще раз, де в каталозі не вказано тип проблеми.

Щоб усунути цю проблему, виконайте наведені нижче дії.

- Переконайтеся, що обліковий запис, який прийняв запрошення електронною поштою, – це той самий обліковий запис, який використовується для входу пізніше. Переконайтеся, що користувач використовує той самий обліковий запис, щоб прийняти запрошення та ввійти на сайт. 

Докладні відомості див. в статті Керування псевдонімами для облікового запису Microsoft для керування [ </a> обліковим Microsoft 365 входу.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Перейдіть до кожного сайту, на якому з'являється повідомлення про помилку. 

Додайте "/_layouts/15/people.aspx/membershipgroupid=0" (у лапках) у кінці URL-адреси сайту. 

Приклад: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Виберіть користувача зі списку.

- Натисніть **кнопку Видалити дозволи користувача на** стрічці. 
-  Поверніть користувача та надайте запрошення користувачу знову.

