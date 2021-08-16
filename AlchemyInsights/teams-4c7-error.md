---
title: Teams 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049329"
---
# <a name="4c7-error-in-microsoft-teams"></a>Помилка 4c7 у Microsoft Teams

Ця помилка виникає, тому що Microsoft Teams вимагає автентифікації форм. Під час розгортання служб об'єднання Active Directory (AD FS) для інтрамережі автентифікацію форм не активовано. Якщо Windows невдала інтегрована автентифікація, буде запропоновано ввійти за допомогою автентифікації форм.

Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою консолі керування AD FS (MMC) на комп'ютері, де є локальна копія Active Directory. Щоб зробити це, виконайте такі дії. 

1. В області переходів перейдіть до пункту Політики **автентифікації.**
2. У розділі **Дії** в області відомостей виберіть Редагувати глобальну **основну автентифікацію.**
3. На вкладці **Інтрамережа** виберіть Автентифікація **форм**.
4. Натисніть **кнопку OK** (або **Застосувати).**