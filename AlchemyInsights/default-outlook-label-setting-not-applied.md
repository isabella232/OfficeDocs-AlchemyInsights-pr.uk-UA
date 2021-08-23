---
title: Стандартне Outlook підпису не застосовано
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455082"
---
# <a name="default-outlook-label-setting-not-applied"></a>Стандартне Outlook підпису не застосовано

Якщо параметри підписів за замовчуванням Outlook застосовуються належним чином і до них не застосовано іншу етикетку або її не застосовано, можливо, виникла відома проблема (MC277818) і для вирішення цієї проблеми потрібно виконати одну з цих двох способів:

**Варіант 1.**

1. Перейдіть у Центр Microsoft 365 відповідності > **захист даних** про  >  **рішення.**
1. Виберіть **політики підписів**, а потім виберіть політику підписів, яку потрібно змінити (**Параметр OutlookDefaultlabel** неправильно налаштовано для потрібної політики підписів. Запустіть **Get-labelpolicy,** щоб переглянути цей параметр), а потім виберіть **Редагувати політику**.
1. Натикайте кнопку Далі, доки не побачите параметр Застосувати  цей стандартний підпис до повідомлень електронної пошти  **,** який доступний, якщо в діалоговому вікні Параметри політики вибрано Вимагати від користувачів застосувати етикетку до електронних листів і документів. 
1. У **діалоговому вікні Застосувати стандартну надпис** до документів виберіть **у** розкривному списку пункт Немає.
1. Натисніть **кнопки Далі** **та Надіслати,** щоб зберегти параметри етикетки.

**Варіант 2.**

У Центрі безпеки та відповідності [PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)за допомогою командлета Set-LabelPolicy **OutlookDefaultlabel** виберіть значення **None** (Немає) в {OutlookDefaultLabel="None"}.

Виконати: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Докладні відомості про стандартні підписи для Outlook див. в цьому [Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)