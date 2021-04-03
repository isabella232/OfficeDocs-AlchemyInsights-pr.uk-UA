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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505731"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Відновлення видаленої групи Microsoft 365

Видалену групу Microsoft 365 або Microsoft Teams можна відновити протягом 30 днів із видалення.

1. Щоб увійти в Центр адміністрування Microsoft 365 і перелічити видалені групи та команди, перейдіть у Центр адміністрування [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)

    **Примітка.** Увійдіть під обліковим записом, призначеним адміністратору-власнику або групі.

1. Виберіть видалену групу Microsoft 365 або Teams, які потрібно відновити, і натисніть **кнопку Відновити групу**.

    Якщо через конфліктну SMTP-адресу не вдається відновити групу, скористайтеся наведеною нижче командою, щоб знайти об'єкт, який призведе до конфлікту, і видаліть SMTP-адресу:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Примітка.** У деяких випадках відновлення групи та всіх її даних може тривати до 24 годин.

    Докладні відомості або про те, як відновити групи за допомогою PowerShell, див. в статті Відновлення видаленої групи [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)