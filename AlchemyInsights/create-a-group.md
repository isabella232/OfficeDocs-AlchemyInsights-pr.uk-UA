---
title: Створення групи
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816393"
---
# <a name="create-a-group"></a>Створення групи

У цій статті описано створення груп.

**Дозвіл на створення групи**

Переконайтеся, що ви маєте право створювати нову групу. Глобальні адміністратори можуть вимкнути створення груп на порталі Azure або на панелі доступу. Може знадобитися адміністратор, щоб створити нову групу для вас або надати вам відповідні дозволи.

**Керування дозволами на створення груп**

1. Глобальні адміністратори можуть керувати дозволами на створення груп (з міркувань безпеки) або групами Office 365, створеними на порталі Azure або панелі доступу, вибравши в розділі "Користувачі можуть створювати групи безпеки на порталах Azure" або "Користувачі можуть створювати групи Office 365 на порталах Azure" в розділі Загальні  >  **групи (параметри)**.
2. Крім того, ви можете обмежити створення груп, щоб вибрати групу користувачів, якщо у вас є ліцензія Azure Active Directory P1 Premium.

**Вимкнення привітання для нових учасників групи Office 365**

Сповіщення про привітання, надіслане користувачам, які додаються до груп Office 365, можна вимкнути, установивши в PowerShell параметр **UnifiedGroupWelcomeMessageEnabled** для False. Відомості про цю настройку [див. тут.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

