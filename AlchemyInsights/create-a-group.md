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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929326"
---
# <a name="create-a-group"></a>Створення групи

У цій статті описано створення груп.

**Дозвіл на створення групи**

Переконайтеся, що ви маєте право створювати нову групу. Глобальні адміністратори можуть вимкнути створення груп на порталі Azure або на панелі доступу. Може знадобитися адміністратор, щоб створити нову групу для вас або надати вам відповідні дозволи.

**Керування дозволами на створення груп**

1. Глобальні адміністратори можуть керувати дозволами на створення груп (з міркувань безпеки) або групами Office 365, створеними на порталі Azure або панелі доступу, вибравши в розділі "Користувачі можуть створювати групи безпеки на порталах Azure" або "Користувачі можуть створювати групи Office 365 на порталах Azure" в розділі Загальні  >  **групи (Настройки)**.
2. Крім того, ви можете обмежити створення груп, вибравши групу користувачів, якщо у вас Azure Active Directory P1 Premium ліцензії.

**Вимкнення привітання для нових Office 365 учасників групи**

Сповіщення про привітання, надіслане користувачам, Office 365 групі, можна вимкнути, установивши в PowerShell параметр **UnifiedGroupWelcomeMessageEnabled** на False. Відомості про цю настройку [див. тут.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

