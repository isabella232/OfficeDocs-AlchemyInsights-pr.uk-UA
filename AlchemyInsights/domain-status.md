---
title: Стан домену – не вибрано жодних служб
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326598"
---
# <a name="domain-status---no-services-selected"></a>Стан домену – не вибрано жодних служб

**Не вибрано жодних** служб означає, що ви не вибрали жодні служби Microsoft 365, як-от Exchange Online, Skype для бізнесу або Intune, а також Керування мобільними пристроями для Microsoft 365 для вашого настроюваного домену. Якщо використовується гібридне середовище Exchange (локальне середовище Exchange із Exchange Online) або зовнішній фільтрування спаму з Exchange без інших служби Microsoft, це повідомлення можна пропустити. Стан справності домену доступний лише для доменів, підключених безпосередньо до служби.

Щоб вибрати служби для домену:

1. На **Настройки** Домени установіть прапорець поруч із доменом, і повідомлення про стан  >  [](https://admin.microsoft.com/Adminportal/Home)Не **вибрано служб.**
1. Виберіть **Manage DNS (Керування службою DNS),** щоб запустити майстер настроювання домену.
    - Якщо ви **виберете Додати власні записи DNS,** виберіть службу, коли з'явиться відповідний запит. Додаткові служби можна знайти в розділі **Додаткові параметри.**
    - Якщо вибрати дозволити **корпорації Майкрософт додавати ваші записи DNS** або Додаткові параметри Настроювання моїх онлайнових служб, усі доступні служби пропонуються та   >   вибираються автоматично.
1. Виконайте всі кроки майстра, щоб завершити настроювання служби DNS і вибрати служби.
 
Додаткову довідку з налаштування домену див. в розділі [Додавання записів DNS для підключення домену.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

