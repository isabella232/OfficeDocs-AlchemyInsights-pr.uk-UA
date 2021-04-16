---
title: Шифрування за допомогою правил транспортування
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813889"
---
# <a name="encryption-with-transport-rules"></a>Шифрування за допомогою правил транспортування

У [Центрі адміністрування Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) для активації шифрування повідомлень можна використовувати можливості шифрування повідомлень Office (OME) у правилах передавання пошти. Виберіть параметр правила транспортування **Застосувати шифрування повідомлень Office 365 і захист прав**.

- Докладні відомості див. в статті [Визначення правила передавання пошти для шифрування](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- У PowerShell скористайтеся командлетом [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) і задайте значення "$true" для параметра *ApplyOME*.
