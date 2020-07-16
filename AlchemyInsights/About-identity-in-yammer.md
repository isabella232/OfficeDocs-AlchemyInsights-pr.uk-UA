---
title: Відомості про посвідчення в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148423"
---
# <a name="about-identity-in-yammer"></a>Відомості про посвідчення в Yammer

Рекомендується, щоб всі мережі, виконайте такі дії, щоб уникнути проблеми, пов'язані з посвідчення:

1. Виконання Office 365 посвідчення після підготовки Microsoft 365 облікових записів для користувачів у Azure AD, щоб переконатися, що всі користувачі ввійти за допомогою їх основний обліковий запис Microsoft 365. Для отримання додаткових відомостей див. [застосування Office 365 посвідчення для користувачів Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Консолідація кількох мереж Yammer. Успадковані конфігурації Yammer дозволяють кільком мережам Yammer для підключення до одного клієнта. Для отримання додаткових відомостей див. у [мережі міграція-консолідація кількох мереж Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Крім того, забезпечити ліцензування Yammer для блокування користувачів з Yammer, якщо вони не мають ліцензії. Для отримання додаткових відомостей див. [керування ліцензіями користувача Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Нарешті, аудит список користувачів для старіших мереж Yammer та призупинення попередніх версій користувачів. Рекомендується призупинити (деактивувати) користувачів, а не видаляти їх, тому що видалення є незворотнім. Щоб отримати додаткові відомості див. [аудит користувачів Yammer в мережах, підключених до Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) і [видалення користувачів](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Настроївши Yammer за допомогою цих дій, ви також будете готові налаштувати мережу Yammer для власного режиму для Microsoft 365. Для отримання додаткових відомостей див. [Настроювання мережі Yammer для власного режиму для Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).