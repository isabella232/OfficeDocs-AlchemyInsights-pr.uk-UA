---
title: Видалення фонової служби для Microsoft Search у службі Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816342"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Видалення фонової служби для Microsoft Search у службі Bing

Щоб видалити фонову службу для Microsoft Search у службі Bing, можна скористатися такими засобами:

1. Щоб повернутися до початкових параметрів пошукової системи, виконайте наведені нижче дії.

    муніципалітет. Установіть перемикач **використовувати Бінг як пошукову програму за замовчуванням [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.

    b. [Перейдіть до центру адміністрування Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) і зніміть параметр, який впливає на всіх користувачів організації.

2. Щоб видалити фонову службу з окремого пристрою, виконайте наведені нижче дії.

    муніципалітет. Виберіть **елемент панель керування > програми > програми та засоби**.

    b. Клацніть правою кнопкою миші **службу Microsoft Search у службі Bing у** списку інстальованих програм, а потім натисніть кнопку **Видалити**.

3. Щоб видалити фонову службу з кількох пристроїв у вашій організації, увійдіть у систему як адміністратор і виконайте таку команду в сценарії: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
