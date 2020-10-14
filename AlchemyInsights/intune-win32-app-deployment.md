---
title: Розгортання програм Win32 (inune)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461997"
---
# <a name="intune-win32-app-deployment"></a>Розгортання програм Win32 (inune)

Microsoft Inune дає змогу використовувати Win32-програми, зокрема, але не обмежуються MSI і. Програма EXE для розгортання пристроїв із Windows 10. Використовуваний механізм розгортання вимагає, щоб на цільовому пристрої було представлено розширення керування Inune (IME). Редактор IME буде автоматично інстальовано в результаті орієнтації на сценарій PowerShell або розгортання програм Win32 для користувача або пристрою.

Також є набір передумов, які потрібно виконати, щоб розгорнути програми Win32, які містять такі елементи:

- Підтримувані платформи: операційна система Windows 10 версії 1607 або пізніша (корпоративні, Pro та навчальні версії).
- Підтримується архітектура: x86 і x64.
- Керування пристроями: під час приєднання до мережі та автоматичної реєстрації (включно з гібридним доменом, до якого приєдналися та групова політика, автоматично зараховані).
- Формат пакетів програм:. файл **intunewin**  , підготовлений за допомогою [засобу підготовчої програми Win32 (Microsoft](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)).
- Обмеження
    - Максимальний розмір: 8GB.
    - Непідтримувана архітектура: озброєння.

Ознайомтеся з документами "[Додавання, призначення та відстеження програми Win32 в Microsoft InTune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" для інформації, пов'язаної з цими кроками.

Докладні відомості про виправлення неполадок розгортання програм у Windows, зокрема програми Win32, можна переглянути в наведених нижче документах.

- [Усунення проблем із інсталяцією програм](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Виправлення неполадок із програмами Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)