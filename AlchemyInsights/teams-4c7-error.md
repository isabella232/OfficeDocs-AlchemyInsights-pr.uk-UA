---
title: Помилка Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786690"
---
# <a name="4c7-error-in-microsoft-teams"></a>Помилка 4c7 у Microsoft Teams

Ця помилка виникає, тому що Microsoft Teams потребує автентифікації форм. Під час розгортання служб об'єднання Active Directory (AD FS) для інтрамережі автентифікацію форм не активовано. Якщо не вдається інтегрована автентифікація Windows, буде запропоновано ввійти за допомогою автентифікації форм.

Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою консолі керування AD FS (MMC) на комп'ютері, де є локальна копія Active Directory. Щоб зробити це, виконайте такі дії. 

1. В області переходів перейдіть до пункту Політики **автентифікації.**
2. У розділі **Дії** в області відомостей виберіть Редагувати глобальну **основну автентифікацію.**
3. На вкладці **Інтрамережа** виберіть Автентифікація **форм**.
4. Натисніть **кнопку OK** (або **Застосувати).**