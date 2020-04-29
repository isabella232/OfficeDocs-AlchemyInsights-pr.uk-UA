---
title: Шифрування за допомогою правил транспортування
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915284"
---
# <a name="encryption-with-transport-rules"></a>Шифрування за допомогою правил транспортування

У [Центрі адміністрування Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) для активації шифрування повідомлень можна використовувати можливості шифрування повідомлень Office (OME) у правилах передавання пошти. Виберіть параметр правила транспортування **Застосувати шифрування повідомлень Office 365 і захист прав**.

- Докладні відомості див. в статті [Визначення правила передавання пошти для шифрування](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- У PowerShell скористайтеся командлетом [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) і задайте значення "$true" для параметра *ApplyOME*.
