---
title: Проблеми з продуктивністю SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911863"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint або OneDrive, недоступні або недоступні для кількох користувачів

SharePoint або OneDrive може бути повільним, недоступним чи недоступним або може відображатися помилка служби недоступна чи 503 – з кількох причин:
  
- Якщо сайт SharePoint або OneDrive повільний або затримується для кількох користувачів, може виникнути тимчасова проблема в службі, через яку під час доступу до веб-сайтів або вмісту SharePoint OneDrive користувачами можуть виникати періодичні затримки або помилки навігації. Перегляньте [приладну дошку справності](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) служби, щоб дізнатися, чи це впливає на вашу організацію.
  
- Користувачі можуть отримати повідомлення *про помилку "503* сервер зайнятий" під час спроби перейти на SharePoint або OneDrive сайтів. Ця помилка може статися через те, що служба SharePoint регуляцію. Служба SharePoint Online використовує дроселювання, щоб забезпечити оптимальну продуктивність і надійність. Дроселювання обмежує кількість дій користувачів або одночасних викликів (за сценарієм або кодом), щоб уникнути надмірного використання ресурсів. Докладні відомості про те, як намагатися це, див. в цій SharePoint [Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Якщо у вас повільна продуктивність класичного або сучасного **SharePoint** сайту або сторінки, проаналізуйте сторінки за допомогою засобу діагностики сторінок.  [](https://aka.ms/perftool)
  
- Якщо продуктивність усе одно низька, перегляньте ресурси в нижній частині цієї статті: Загальні відомості про підвищення продуктивності для SharePoint [Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  