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
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887461"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Індикатори не працюють у браузері Edge

Після створення індикатора межа (Smartscreen) не вражується. Докладні відомості див. [в розділі Створення індикаторів для IPs, URL-адрес або доменів.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Крок 1. Переконайтеся, що:

- Переконайтеся, що індикатор правильний (неправильно введено IP-адресу або URL-адресу, правильні дії, правильні групи RBAC).
- Зачекайте 2 години після створення індикатора, щоб врахувати будь-яку можливу затримку.
- Переконайтеся, що систему до'єднано до Microsoft Defender для кінцевої точки.
- Переконайтеся, що системи можуть спілкуватися з хмарою.
- Переконайтеся, що фільтр Smartscreen увімкнуто й доступний, перейшовте на [тестовий сайт.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Крок 2. Усунення потенційної проблеми

- Переконайтеся, що клієнт відповідає вимогам. Докладні відомості [див. в розділі Створення індикаторів для IPs, URL-адрес або доменів.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Переконайтеся, що ви використовуєте найновішу версію браузера Edge. Відомості про те, як дізнатися останню версію, див. в [Microsoft Edge.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Перезапустіть браузер Edge.
- Перейдіть на сайт, для якого налаштоться індикатор. Якщо сайт відображається ненадійно, перейдіть до кроку 3. 

## <a name="step-3-collect-data"></a>Крок 3. Збирання даних

- Збирати **діагностичні дані MDEClientAnalyzer.** Інструкції див. в [статті Проблеми з приєднуванням до Microsoft Defender для кінцевої точки.](issues-with-onboarding-machines.md)
- Якщо ви вмієте інсталювати й збирати трасування Fiddler, див. дія програми [Telerik Fiddler.](http://www.telerik.com/fiddler)
- Якщо ви віддаєте перевагу інструкціям від служби підтримки Microsoft, клацніть піктограму підтримки нижче, щоб відкрити інцидент служби підтримки.
