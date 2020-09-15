---
title: 646 як настроїти AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704510"
---
# <a name="configure-sync-features"></a>Настроювання функцій синхронізації

Azure AD Connect містить кілька функцій, які ввімкнуто за замовчуванням, або які можна ввімкнути згодом. Деякі функції потребують додаткової конфігурації в певних середовищах.

- [Фільтрування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обмежує об'єкти, синхронізовані з ЛАЗУРОЧНИМ оголошенням. За замовчуванням для всіх користувачів, контактів, груп і комп'ютерів із Windows 10 синхронізуються облікові записи. Ви можете включити або виключити об'єкти на основі доменів, OUs та інших атрибутів.

- [Синхронізація гешування паролів](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронізує хеш пароля з локального Active Directory на ЛАЗУРНЕ AD. Це дає змогу керувати паролем в одному розташуванні, але використовувати той самий пароль в локальних і хмарних середовищах. Оскільки служба Active Directory – це авторитетний джерело, ви можете використовувати власні політики паролів.

- Для [самостійного скидання пароля (sspr)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) користувачі можуть скинути власні паролі в хмарі, а також застосовувати локальну політику паролів.

- [Пристрій writback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) дає змогу реєструвати пристрої в AZURE AD, які повертаються в локальну службу Active Directory, щоб їх можна було використовувати для умовного доступу.

- [Запобігання випадковому вилученням](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) за замовчуванням для запобігання занадто багатьох одночасних видалень об'єктів (понад 500 об'єктів на синхронізацію). Ви можете змінити цей параметр, щоб відповідно до потреб вашої організації.

- [Автоматичне оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) активовано за замовчуванням для Експрес-інсталяцій і допомагає забезпечити свою версію AZURE AD Connect завжди поточна.
