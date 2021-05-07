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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233534"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>Помилка 401 Несанкціоноване SharePoint

Якщо в програмі SharePoint відображається повідомлення про помилку "(401) Неавторизовано" може бути пов'язано з вилученням протоколу TLS 1.0/1.1. Докладні відомості:

[Підготовка до TLS 1.2 у Office 365 і Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Помилки автентифікації, якщо клієнт не підтримує протокол TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Якщо користувачів увімкнено Windows 7, переконайтеся, що вони перевіряли [TLS Cipher Suites Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)