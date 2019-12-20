---
title: Команди 4C7 Error
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796456"
---
# <a name="4c7-error-in-microsoft-teams"></a>4C7 помилка в Microsoft teams

Ця помилка виникає через те, що Microsoft teams потребує автентифікації форм. Під час розгортання служби Active Directory об'єднання Services (AD FS), форми автентифікації не ввімкнуто для інтрамережі за промовчанням. Якщо не вдається виконати інтегровану автентифікацію Windows, буде запропоновано ввійти за допомогою форм автентифікації.

Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою оснащення AD FS консолі керування Microsoft (MMC) на комп'ютері, який має локальну копію служби Active Directory. Щоб зробити це, виконайте такі дії. 

1. В області переходів перейдіть до **політики автентифікації**.
2. У розділі **дії** в області відомостей виберіть пункт **редагувати глобальний первинний автентифікації**.
3. На вкладці **інтрамережі** виберіть **автентифікацію форм**.
4. Виберіть **OK** (або **Застосувати**).