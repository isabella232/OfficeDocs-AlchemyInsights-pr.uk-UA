---
title: Індикатори не працюють у браузері Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676575"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Індикатори не працюють у браузері Edge

Якщо ви створили індикатор, його не вражено в Edge (фільтр Smartscreen). Докладні відомості див. [в розділі Створення індикаторів для IPs, URL-адрес або доменів.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Крок 1. Переконайтеся, що:

- Переконайтеся, що індикатор правильний (неправильно введено IP-адресу або URL-адресу, правильні дії, правильні групи RBAC).
- Зачекайте 2 години після створення індикатора, щоб врахувати будь-яку можливу затримку.
- Переконайтеся, що систему до'єднано до Microsoft Defender для кінцевої точки.
- Переконайтеся, що системи можуть спілкуватися з хмарою.
- Переконайтеся, що фільтр Smartscreen увімкнуто й доступний, перейшовте на [тестовий сайт.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Крок 2. Усунення потенційної проблеми

- Переконайтеся, що клієнт відповідає вимогам. Докладні відомості [див. в розділі Створення індикаторів для IPs, URL-адрес або доменів.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Переконайтеся, що ви використовуєте найновішу версію браузера Edge. Відомості про те, як дізнатися останню версію, див. в [Microsoft Edge.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Перезапустіть браузер Edge.
- Перейдіть на сайт, для якого налаштоться індикатор. Якщо сайт відображається ненадійно, перейдіть до кроку 3. 

## <a name="step-3-collect-data"></a>Крок 3. Збирання даних

- Збирати **діагностичні дані MDEClientAnalyzer.** Інструкції див. в [статті Проблеми з приєднуванням до Microsoft Defender для кінцевої точки.](issues-with-onboarding-machines.md)
- Якщо ви вмієте інсталювати й збирати трасування Fiddler, див. дія програми [Telerik Fiddler.](http://www.telerik.com/fiddler)
- Якщо ви віддаєте перевагу інструкціям від служби підтримки Microsoft, клацніть піктограму підтримки нижче, щоб відкрити інцидент служби підтримки.
