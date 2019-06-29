---
title: 646 як налаштувати AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385401"
---
# <a name="configure-sync-features"></a>Настроювання синхронізації функцій

Блакитні оголошення підключення включає кілька функцій, що включений за замовчуванням або яку можна ввімкнути пізніше. Деякі функції вимагають додаткових налаштувань в конкретних умовах.

- [Фільтрування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) межі об'єкти синхронізуються блакитні оголошення. За замовчуванням, всі користувачі, контакти, групи та версії 10 синхронізуються комп'ютер облікових записів. Ви можете додати або вилучити об'єктів на основі доменів, підрозділи та інші атрибути.

- [Синхронізація геш пароля](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронізація пароля хеш із локальної служби Active Directory до блакитні оголошення. Це дозволяє Керування паролями в одному місці, але використовувати однаковий пароль в обох локальні та хмарними. Тому, що Active Directory надійного джерела, ви можете використовувати свій власний політики паролів.

- [Скидання пароля самообслуговування (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) дозволяє користувачам можливість скидати паролі у хмарі при застосуванні як і раніше ваш пароль локальною політикою.

- [Пристрій writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) надає змогу зареєстрованим у блакитній оголошення, щоб записати назад до локальної служби Active Directory так що вони можуть бути використані для умовного доступу.

- [Випадкове ю видалення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ввімкнуто за промовчанням, щоб запобігти забагато видалень синхронний об'єкта (більш ніж 500 об'єктів на синхронізацію). Можна змінити цей параметр для задоволення потреб вашої організації.

- [Автоматичні оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ввімкнуто за промовчанням для Експрес установок і допомагає забезпечити вашу версію Azure оголошення Коннект актуальний завжди.
