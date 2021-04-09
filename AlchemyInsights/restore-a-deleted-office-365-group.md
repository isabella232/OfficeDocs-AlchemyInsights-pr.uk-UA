---
title: Відновлення видаленої групи Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645152"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Відновлення видаленої групи Microsoft 365

Видалену групу Microsoft 365 або Microsoft Teams можна відновити протягом 30 днів із видалення.

1. Перейдіть до [Центру адміністрування Microsoft 365,](https://aka.ms/RestoreDeletedGroup) щоб увійти в список видалених груп і команд.

    **Примітка.** Увійдіть під обліковим записом, призначеним адміністратору-власнику або групі.

1. Виберіть видалену групу Microsoft 365 або Teams, які потрібно відновити, і натисніть **кнопку Відновити групу**.

    Якщо через конфліктну SMTP-адресу не вдається відновити групу, скористайтеся наведеною нижче командою, щоб знайти об'єкт, який призведе до конфлікту, і видаліть SMTP-адресу:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Примітка.** У деяких випадках відновлення групи та всіх її даних може тривати до 24 годин.

    Докладні відомості або про те, як відновити групи за допомогою PowerShell, див. в статті Відновлення видаленої групи [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)