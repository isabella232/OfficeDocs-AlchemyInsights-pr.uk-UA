---
title: Видалити загублений користувача з локального сервера
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198583"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Видалити загублений користувача з локального сервера

Щоб видалити загублений користувача, виконайте такі дії:

1. Примусове синхронізації каталогів, слідуючи інструкціям в [тому, що таке Гібридна ідентичність з Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Щоб перевірити синхронізацію каталогів, подивіться, [що таке Гібридна ідентичність з Active Directory Azure?](https://technet.microsoft.com/library/jj151797.aspx).

3. Якщо функція синхронізації належним чином, але видалення об'єкта Active Directory не поширюється на Azure AD, вручну видалити загублений об'єкт за допомогою одного з таких Azure Active Directory модуль для командлети оболонки Windows PowerShell:

    Видалити-MsolContact  
    Видалити-MsolGroup  
    Видалення MsolUser

    Наприклад, щоб видалити загублений ІДЕНТИФІКАТОР користувача john.smith@contoso.com, спочатку створеного за допомогою синхронізації каталогів, запустіть командлет:

    Видалення MsolUser – ім'я користувача John.Smith@Contoso.com