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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830054"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Мікрозатримки та дроселювання в Exchange Online PowerShell

Під час запуску сценаріїв і командлетів в Exchange Online можуть виникати затримки або відображатися попередження "Застосовано мікрозатримку". Ось дві поради щодо цього:

- Можливо, слід спробувати [модуль Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), що включає командлети, засновані на REST API та значно продуктивніші. Це рішення може чудово підійти для багатьох командлетів Get-, що часто використовуються.
- Якщо вам потрібно використовувати командлети, яких ще немає модуля v2, ознайомтеся зі статтею [Виконання командлетів PowerShell для великих кількостей користувачів в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), у якій обговорюються способи обходу очікуваних обмежень дроселювання PowerShell в Exchange Online.
