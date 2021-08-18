---
title: Установіть для параметра ClientAccessServerEnabled значення True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320377"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Установіть для параметра ClientAccessServerEnabled значення True

Якщо ви не можете відкрити зашифроване повідомлення електронної пошти, а натомість бачите вкладення **rpmsg,** виконайте такі дії:

1. Підключення, щоб Exchange Online PowerShell.

    **Примітка.** Щоб підключитися Exchange Online PowerShell, потрібно ввійти, використовуючи обліковий запис глобального адміністратора Exchange адміністратора.

   a. Відкрийте Windows PowerShell а потім виконайте таку команду:`$UserCredential = Get-Credential`
   b. У **діалоговому вікні Windows PowerShell облікових** даних введіть свій робочий або навчальний обліковий запис і пароль, в. Натисніть кнопку **OK**. 

2. Щоб створити новий сеанс, виконайте таку команду:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Запустіть таку команду:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Виконати `Get-IRMConfiguration` команду.

4. Перевірте **параметр ClientAccessServerEnabled.** 

    a. Якщо **для параметра ClientAccessServerEnabled** установлено **значення False,** запустіть такий командлет: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Порада.** Завжди закривайте сеанс PowerShell за допомогою такої команди: `Remove-PSSession $Session`

Докладні відомості див. в [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

