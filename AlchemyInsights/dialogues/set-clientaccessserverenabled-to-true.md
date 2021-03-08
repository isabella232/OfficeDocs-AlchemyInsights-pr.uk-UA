---
title: Настроювання значення "для сервера"
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527416"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Настроювання значення "для сервера"

Якщо ви не можете відкрити зашифроване повідомлення електронної пошти, а натомість побачити вкладення **rрmsg** , виконайте наведені нижче дії.

1. Підключіться до Exchange Online PowerShell.

> [!NOTE]
> Щоб підключитися до служби Exchange Online PowerShell, потрібно ввійти за допомогою глобального адміністратора або облікового запису Exchange адміністратора.

   муніципалітет. Відкрийте Windows PowerShell, а потім виконайте таку команду: `$UserCredential = Get-Credential`
b. У діалоговому вікні **запит облікових даних Windows PowerShell** введіть свій робоча або навчальний обліковий запис і пароль, c. Натисніть кнопку **OK**. 

2. Щоб створити новий сеанс, виконайте таку команду:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    муніципалітет. Запустіть таку команду:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Команда «виконати `Get-IRMConfiguration` ».

4. Установіть прапорець поруч із параметром **Clienacc"** . 

    муніципалітет. Якщо параметр **Clienacceserverenувімкнуто** , установлено значення **false**, запустіть наведений нижче командлет. `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Завжди закривайте сеанс PowerShell за допомогою наведеної нижче команди. `Remove-PSSession $Session`

Докладні відомості наведено в статті [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

