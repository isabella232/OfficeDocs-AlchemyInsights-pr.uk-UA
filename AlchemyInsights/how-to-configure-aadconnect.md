---
title: 646 як налаштувати AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722584"
---
# <a name="configure-sync-features"></a>Настроювання функцій синхронізації

Azure AD-підключення, містить кілька функцій, які ввімкнуто за промовчанням або можна ввімкнути пізніше. Деякі функції потребують додаткової конфігурації в певних середовищах.

- [Фільтрування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обмеження об'єкти СИНХРОНІЗУЮТЬСЯ Azure AD. За промовчанням синхронізуються всі користувачі, контакти, групи та комп'ютерні облікові записи Windows 10. Можна включити або виключити об'єкти на основі доменів, OUs або інших атрибутів.

- [Геш-синхронізація пароля](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронізує геш-пароль з локальної служби Active Directory для Azure AD. Це дозволяє Керування паролями в одному розташуванні, але використання одного і того ж пароля в локальних і хмарних середовищах. Оскільки Active Directory є авторитетним джерелом, ви можете використовувати свої власні політики паролів.

- [Самостійне скидання пароля (sсрп)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) дозволяє користувачам скидати свої власні паролі в хмарі, а ще застосування вашої локальної політики паролів.

- [Пристрій writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) дозволяє зареєстровані пристрої в Azure AD, щоб бути написана на локальному Active Directory, щоб вони могли бути використані для умовного доступу.

- [Запобігання випадковому видалення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) увімкнуто за промовчанням, щоб запобігти занадто багато одночасних видалення об'єктів (більше 500 об'єктів на синхронізацію). Ви можете змінити цей параметр, щоб задовольнити потреби вашої організації.

- [Автоматичне оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) увімкнуто за промовчанням для Експрес-інсталяції та гарантує, що ваша версія Azure AD-підключення завжди поточного.
