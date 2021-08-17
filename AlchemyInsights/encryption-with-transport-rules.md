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
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079471"
---
# <a name="encryption-with-transport-rules"></a>Шифрування за допомогою правил транспортування

У [Центрі адміністрування Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) для активації шифрування повідомлень можна використовувати можливості шифрування повідомлень Office (OME) у правилах передавання пошти. Виберіть параметр правила транспортування **Застосувати шифрування повідомлень Office 365 і захист прав**.

- Докладні відомості див. в статті [Визначення правила передавання пошти для шифрування](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- У PowerShell скористайтеся командлетом [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) і задайте значення "$true" для параметра *ApplyOME*.
