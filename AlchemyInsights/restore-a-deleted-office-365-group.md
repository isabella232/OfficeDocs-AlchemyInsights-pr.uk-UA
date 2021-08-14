---
title: Відновлення видаленої Microsoft 365 групи
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959047"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Відновлення видаленої Microsoft 365 групи

Видалену групу або Microsoft 365 видалити Microsoft Teams протягом 30 днів із видалення.

1. Перейдіть до [Центр адміністрування Microsoft 365,](https://aka.ms/RestoreDeletedGroup) щоб увійти до списку видалених груп і команд.

    **Примітка.** Увійдіть під обліковим записом, призначеним адміністратору-власнику або групі.

1. Виберіть видалену Microsoft 365 або групу Teams які потрібно відновити, і натисніть кнопку **Відновити групу**.

    Якщо через конфліктну SMTP-адресу не вдається відновити групу, скористайтеся наведеною нижче командою, щоб знайти об'єкт, який призведе до конфлікту, і видаліть SMTP-адресу:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Примітка.** У деяких випадках відновлення групи та всіх її даних може тривати до 24 годин.

    Докладні відомості або про те, як відновити групи за допомогою PowerShell, див. в статті Відновлення [видалених груп Microsoft 365 груп.](https://go.microsoft.com/fwlink/?linkid=867802)