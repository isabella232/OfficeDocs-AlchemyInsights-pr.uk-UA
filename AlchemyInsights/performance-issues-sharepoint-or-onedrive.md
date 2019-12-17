---
title: Проблеми продуктивності-SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068442"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint або OneDrive, повільно, недоступний або недоступний для кількох користувачів

SharePoint або OneDrive можуть бути повільними, недоступними або недоступні, або може відображатися Служба недоступна або 503 помилки, з кількох причин:
  
- Якщо ваш сайт SharePoint або OneDrive уповільнюється або затримується для кількох користувачів, може виникнути проблема тимчасового обслуговування, коли користувачі відчувають періодичні затримки або помилки навігації під час доступу до сайтів SharePoint або вмісту OneDrive. Перегляньте [приладну дошку стану служби](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.
  
- Користувачі можуть отримувати *503 сервер зайнятий* , помилка під час спроби перейти до SharePoint або OneDrive сайтів. Ця помилка може бути викликана дроселювання у службі SharePoint. SharePoint Online використовує дроселювання для підтримки оптимальної продуктивності та надійності служби SharePoint Online. Дроселювання обмежує кількість дій користувача або одночасних викликів (за сценарієм або кодом) для запобігання надмірного використання ресурсів. Для отримання додаткових відомостей про дроселювання можна [уникнути обмеження або блокування в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Якщо спостерігається низька швидкодія за допомогою **класичного** або **сучасного** сайту SharePoint або сторінки, використовуйте [засіб діагностики сторінок](https://aka.ms/perftool) для аналізу сторінок.
  
- Якщо ви все ще відчуваєте загальне зниження продуктивності, будь ласка, перегляньте ресурси в нижній частині цієї статті: [вступ до налаштування продуктивності для SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  