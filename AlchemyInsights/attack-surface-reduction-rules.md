---
title: Правила зменшення поверхні атаки
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676569"
---
# <a name="attack-surface-reduction-rules"></a>Правила зменшення поверхні атаки

Виключаючи файли або папки, можна серйозно зменшити захист, передбачений правилами зменшення поверхні атаки. Файли, які заблокував би правило, дозволено запускати, і звіти або події не записуються. Виняток поширюється на всі правила, які дозволяють винятки.

Виключення ASR використовують такий самий синтаксис, як Антивірус для Microsoft Defender винятки. Докладні відомості [див. в Антивірус для Microsoft Defender перевірки винятків.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Щоб уникнути проблем, перегляньте типові помилки, яких слід уникати під час визначення [винятків.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Винятки підтримуються не в усіх правилах ASR. Щоб перевірити, чи підтримує правило винятки, див. таблицю Правила зменшення поверхні [атаки](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Правила зменшення поверхні атаки

Поверхня атаки вашої організації включає в себе всі місця, де зловмисник може компромісувати пристрої або мережі організації. Зменшення поверхні атаки означає захист пристроїв і мережі організації, що залишає зловмисників меншою кількості способів виконання атак. Може допомогти налаштувати правила зменшення поверхні атаки в Microsoft Defender для кінцевої точки.

Докладні відомості:

- [Зіставлення GUID правила ASR з іменем](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Вимоги до правил asR:
    - [Windows 10 Pro версії 1709 або пізнішої](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise версії 1709 або пізнішої](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, версія 1803 (щопіврічний канал оновлення) або пізніша](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Визначення правильного винятку для застосування

1. Знайдіть ідентифікатор події 1121 або 1122 в журналі Microsoft-Windows-Захисник Windows/Operational.

1. Оцініться сценарій блокування та контекст і переконайтеся, що цей сценарій потрібно розблокувати.

1. Прочитайте значення Шлях у докладних відомостей про подію ( це значення, яке визначає виняток).
    - Зробіть виняток якомога строгим.
    - За потреби застосуйте символ узагальлення (наприклад, замінити змінну користувача).

1. Застосуйте винятки відповідно до своїх потреб у розгортанні. Докладні відомості див. в [розділі Налаштування правил зменшення поверхні атаки](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Виняток не дотримується

1. Визначте, чи підтримує правило винятки. Докладні відомості див. в [правилах зменшення поверхні атаки](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Перегляньте винятки, що застосовуються, і перевірте, чи введено неправильно введені або неправильно інтерпретовані символи узагальнення. Докладні відомості див. в [розділах Підтримувані типи винятку](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. якщо вплив правила воно задовге, спробуйте перемістити правило (назад) у режим перевірки, щоб виконати подальшу перевірку. Докладні відомості див. в [статті Перевірка роботи функцій кінцевої точки в](/microsoft-365/security/defender-endpoint/audit-windows-defender)Microsoft Defender в режимі аудиту.

1. Зберіть дані служби підтримки, щоб відкрити інцидент служби підтримки за допомогою цієї команди:
    
   ** MDEClientAnalyzer.cmd -v**

    Докладні відомості див. в статті Проблеми з приєднуванням [до Захисника Microsoft Для кінцевих точок.](issues-with-onboarding-machines.md)
