---
title: Проблеми з входом у Microsoft 365 програми
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744667"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Проблеми з входом у Програми Microsoft 365

Примітка. Якщо ви використовуєте попередню версію Windows (наприклад, Windows 7 із пакетом оновлень 1 (SP1), Windows [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Server 2008 R2), скористайтеся засобом простого виправлення, щоб увімкнути TLS 1.2 за замовчуванням. Докладні відомості див. в статтях Оновлення для ввімкнення [протоколів TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)як безпечних протоколів за замовчуванням у WindowsHTTP у Windows.

Щоб вирішити проблеми із входом у програми Microsoft 365, спробуйте виконати такі дії на відповідному комп'ютері:  

- Докладні Windows див. в Рекомендації вирішення поширених проблем [із входом.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Відомості для комп'ютерів Mac див. в статтях Не вдається ввійти в [програму Office 2016 для Mac.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Порада.** На комп’ютерах із Windows ми можемо діагностувати та автоматично усунути кілька поширених проблем із входом у систему Office. Завантажте та запустіть  **[Помічник із підтримки й відновлення від Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**, щоб скористатися нашим автоматизованим інструментом.

**Примітка.** Не рекомендовано вимикати сучасну автентифікацію (ADAL) або керування веб-обліковими записами (WAM) для вирішення проблем із входом або **активацією.** Якщо під час підключення до Microsoft 365 за допомогою Office 2013 виникають [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) помилки, активуйте сучасну автентифікацію для Office клієнта.

Конкретні дії з виправлення неполадок див. в перенесеннях:

[Проблеми з входом після оновлення до Office 2016 збірки 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Не вдається ввійти у свій обліковий запис, виданий організацією, наприклад Office 365, Azure або Intune.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Усунення несправностей, пов'язаних із програмами, не пов'язаними з браузерами, які не Office 365, Azure або Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Неодноразово з'являється запит на введення облікових даних Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)