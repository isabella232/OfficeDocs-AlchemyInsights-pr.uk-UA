---
title: 646 Налаштування AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963664"
---
# <a name="configure-sync-features"></a>Настроювання функцій синхронізації

Azure AD Підключення містить кілька функцій, увімкнутих за замовчуванням, або які можна ввімкнути пізніше. Для деяких функцій потрібна додаткова конфігурація в певних середовищах.

- [Фільтрування обмежує](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) кількість об'єктів, які синхронізуються з Azure AD. За замовчуванням синхронізуються всі користувачі, контакти, групи Windows 10 комп'ютера. Ви можете додати або виключити об'єкти на основі доменів, OUs або інших атрибутів.

- [Синхронізація гешування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) паролів синхронізує гешування паролів із локальної служби Active Directory з Azure AD. Це дає змогу здійснювати керування паролями в одному розташуванні, але використовувати один і той самий пароль у локальному й хмарному середовищах. Оскільки Active Directory – важливе джерело, можна використовувати власні політики паролів.

- [Самостійне скидання пароля (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) дає користувачам змогу скидати власні паролі в хмарі, застосовуючи політику локального пароля.

- [Записування пристроїв](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) дає змогу записувати зареєстровані пристрої в Azure AD в локальну каталог Active Directory, щоб їх можна було використовувати для умовного доступу.

- [За замовчуванням функцію запобігання](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) випадковому видаленню ввімкнуто, щоб запобігти забагато видалення одночасного об'єкта (понад 500 об'єктів на синхронізацію). Цей параметр можна змінити відповідно до потреб організації.

- [Автоматичне](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) оновлення ввімкнуто за замовчуванням для швидких інсталяцій і гарантує, що версія Azure AD Підключення завжди актуальна.
