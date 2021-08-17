---
title: Помилка 401 Несанкціоноване SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890287"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>Помилка 401 Несанкціоноване SharePoint

Якщо в програмі SharePoint'являється повідомлення про помилку "(401) Неавторизовано" може бути пов'язано з вилученням протоколу TLS 1.0/1.1. Докладні відомості:

- [Підготовка до TLS 1.2 у Office 365 і Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Помилки автентифікації, якщо клієнт не підтримує протокол TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Оновлення для ввімкнення TLS 1.1 і TLS 1.2 як безпечних протоколів за замовчуванням у WindowsHTTP у Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Якщо користувачів увімкнено Windows 7, переконайтеся, що вони перевіряли [TLS Cipher Suites Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)