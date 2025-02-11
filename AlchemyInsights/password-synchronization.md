---
title: Синхронізація пароля
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960856"
---
# <a name="password-synchronization"></a>Синхронізація пароля

**Синхронізація гешування паролів взагалі не працює**

Коли синхронізація гешування паролів не працює, можуть виникнути деякі поширені проблеми.

- Обліковий запис Active Directory, який використовується в Azure AD Підключення для спілкування  з локальною  службою Active Directory, не надає змін у службі реплікації каталогів і змін у каталозі реплікації всіх дозволів, необхідних для синхронізації паролів. Щоб виправити це, надайте ці дозволи обліковому запису Active Directory.
- Синхронізація гешування паролів вимикається, якщо  адміністратор змінив метод "Користувач Sign-In" з синхронізації паролів на інший параметр, наприклад Федерацію з  **AD FS** у майстрі Azure AD Підключення– щоб виправити це, повторно ввімкніть функцію синхронізації гешування паролів у майстрі Azure AD Підключення.
- Проблема з підключенням до локальної служби Active Directory. Наприклад, деякі контролери домену недоступні в Azure AD Підключення, [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) а порти, необхідні, блокуються брандмауером. Це потрібно виправити, перевіривши правильність підключення між сервером Azure AD Підключення і локальною службою Active Directory.
- Сервер Azure AD Підключення зараз перебуває в режимі розміщення, що призведе до того, що сервер не може вдатися до шахраїв паролів . Щоб усунути цю проблему, виконайте кроки, описані в розділі Виправлення неполадок синхронізації паролів за допомогою синхронізації Azure AD Підключення – Паролі не [синхронізуються.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Синхронізація гешування паролів не працює для деяких користувачів**

1. Якщо ви виявили, що гешування паролів  не синхронізується для користувача, скористайтеся завданням виправлення неполадок в Azure AD Підключення, щоб дослідити та вирішити цю проблему. Виконайте такі завдання:

    a. [Запуск завдання виправлення неполадок у майстрі](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Скористайтеся командлетом виправлення неполадок, щоб дослідити проблему синхронізації гешування паролів для певного використання](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Локальний об'єкт користувача Active Directory активовано для користувача має змінити пароль під час **наступного входу.** Якщо цей параметр увімкнуто, користувачу призначається тимчасовий пароль, який буде запропоновано змінити під час наступного входу. Azure AD Підключення не синхронізує тимчасові паролі з Azure AD.

Щоб вирішити наведену вище проблему, виконайте одну з таких дій:

- Попросіть користувача ввійти в локальну програму (наприклад, Windows робочий стіл) і змінити пароль. Новий пароль буде синхронізовано з Azure AD.
- Адміністратор може оновити пароль користувача, не вмикаючи параметр, Користувач повинен змінити пароль під час наступного входу та надати користувачу спільний доступ до нового пароля. 

3. Локальний об'єкт active Directory User налаштовано неправильно для синхронізації **об'єктів** або синхронізації паролів. Щоб усунути цю проблему, виконайте кроки, описані в статті Усунення несправностей із синхронізацією гешування паролів [за допомогою Azure AD Підключення синхронізації.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







