---
title: Мікрозатримки та дроселювання в Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314721"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Мікрозатримки та дроселювання в Exchange Online PowerShell

Під час запуску сценаріїв і командлетів в Exchange Online можуть виникати затримки або відображатися попередження "Застосовано мікрозатримку". Нижче наведено кілька порад, як вирішити цю проблему.

- Запустіть нашу діагностику, щоб розслабити політики дроселювання PowerShell свого клієнта. Це рішення дасть вам найбільше вирішувати проблему.
- Якщо проблему все одно не вдалося вирішити, скористайтеся [модулем PowerShell Exchange Online версія 2,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)до якого входять командлети на основі REST API, які значно ефективніші. Це рішення може чудово підійти для багатьох командлетів Get-, що часто використовуються.
- Якщо потрібно використовувати командлети, які не описано в модулі v2, див. статті Запуск [командлетів PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)для великої кількості користувачів у Office 365, у яких йдеться про те, як обійти обмеження дроселювання PowerShell у Exchange Online.
