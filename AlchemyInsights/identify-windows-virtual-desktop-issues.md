---
title: Визначення проблем із віртуальним робочим столом Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596038"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Визначення проблем із віртуальним робочим столом Windows

У службі діагностики віртуальних робочих столів Windows використовується лише один командлет PowerShell, але містить багато необов'язкових параметрів, щоб усунути й усунути проблеми. Початок роботи 

1. Завантажте та імпортуйте модуль PowerShell для Windows Virtual Desktop. Докладні відомості див. в [командлетах Windows Virtual Desktop для Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Щоб увійти у свій обліковий запис, запустіть цей командлет:
    
    Приклад: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**ПРИМІТКА.** Усі запити, які використовують PowerShell, мають містити параметри -UserName або -ActivityID. Відомості про можливості моніторингу див. в відомості про використання аналітики журналів для [функції діагностики.](https://go.microsoft.com/fwlink/?linkid=2126847)

Щоб відфільтрувати дії діагностики за користувачем, запустіть такий командлет:

Приклад: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Щоб виявити проблеми, можна запустити список фільтрів. Докладні відомості про діагностування неполадок див. в статтях [Визначення та діагностування проблем із віртуальним робочим столом Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Докладні відомості про поширені помилки див. в [статтях Загальні помилки senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
