---
title: Проблеми з SharePoint на Windows 7 комп'ютерах
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125781"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Проблеми з SharePoint на Windows 7 комп'ютерах

Якщо під час роботи з SharePoint або OneDrive на комп'ютерах Windows 7 з'являться помилки, можливо, вони пов'язані з вилученням протоколу TLS 1.0/1.1. Докладні відомості:

- [Підготовка до TLS 1.2 у Office 365 і Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows клієнтів із пакетом оновлень 1 (SP1 Windows 8 7 і Windows 8 має бути активовано TLS1.2. Докладні відомості див. в описі помилок автентифікації, коли клієнт не підтримує [TLS 1.2.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Інсталюйте оновлення KB3140245 і створіть значення реєстру. Докладні відомості див. в статтях Оновлення для ввімкнення [протоколів TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) як безпечних протоколів за замовчуванням у WindowsHTTP у Windows

- Windows клієнти з пакетом оновлень 1 (SP1 Windows 8 7 і Windows 8 мають інсталювати найновіші програмні комплекси шифрів TLS. Докладні відомості див. в статті Поради з безпеки [Microsoft 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


