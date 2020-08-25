---
title: Відправник не отримає повідомлення електронної пошти, надіслане до групи Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872298"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Відправник не отримає повідомлення електронної пошти, надіслане до групи Microsoft 365

За замовчуванням Відправник повідомлення електронної пошти до групи Microsoft 365 не отримує копії повідомлення в папці "Вхідні", навіть якщо відправник – учасник групи.

Використовуйте цю команду EXO PowerShell, щоб відправник міг отримувати копії кожного повідомлення електронної пошти, які вони надсилають до групи Microsoft 365.  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Щоб увімкнути параметр для всіх поштових скриньок одночасно, зробіть ось що.

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Примітка** . Зміни, внесені до цього параметра, займають значення години, щоб вони набрали сили.