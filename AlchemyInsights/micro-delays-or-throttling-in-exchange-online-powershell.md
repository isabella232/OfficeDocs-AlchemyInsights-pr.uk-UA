---
title: Мікрозатримки та дроселювання в Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948026"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Мікрозатримки та дроселювання в Exchange Online PowerShell

Під час запуску сценаріїв і командлетів в Exchange Online можуть виникати затримки або відображатися попередження "Застосовано мікрозатримку". Ось дві поради щодо цього:

- Можливо, слід спробувати [модуль Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), що включає командлети, засновані на REST API та значно продуктивніші. Це рішення може чудово підійти для багатьох командлетів Get-, що часто використовуються.
- Якщо вам потрібно використовувати командлети, яких ще немає модуля v2, ознайомтеся зі статтею [Виконання командлетів PowerShell для великих кількостей користувачів в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), у якій обговорюються способи обходу очікуваних обмежень дроселювання PowerShell в Exchange Online.
