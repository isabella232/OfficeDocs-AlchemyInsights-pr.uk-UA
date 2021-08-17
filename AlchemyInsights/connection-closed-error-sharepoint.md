---
title: Помилка закриття основного підключення в SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883340"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Помилка "Основне підключення закрито" в SharePoint

Якщо в програмі SharePoint відображається повідомлення про помилку "Основне підключення закрито", можливо, воно пов'язане з вилученням протоколу TLS 1.0/1.1. Докладні відомості див. в таких статтях:

- [Підготовка до TLS 1.2 у Office 365 і Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Помилки автентифікації, якщо клієнт не підтримує протокол TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Оновлення для ввімкнення протоколів TLS 1.1 і TLS 1.2 як безпечних протоколів за замовчуванням у WindowsHTTP у Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Якщо користувачів увімкнено Windows 7, переконайтеся, що вони перевіряли [TLS Cipher Suites Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)