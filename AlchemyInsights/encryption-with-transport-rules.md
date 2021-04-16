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
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="8a694-102">Шифрування за допомогою правил транспортування</span><span class="sxs-lookup"><span data-stu-id="8a694-102">Encryption with transport rules</span></span>

<span data-ttu-id="8a694-103">У [Центрі адміністрування Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) для активації шифрування повідомлень можна використовувати можливості шифрування повідомлень Office (OME) у правилах передавання пошти.</span><span class="sxs-lookup"><span data-stu-id="8a694-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="8a694-104">Виберіть параметр правила транспортування **Застосувати шифрування повідомлень Office 365 і захист прав**.</span><span class="sxs-lookup"><span data-stu-id="8a694-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="8a694-105">Докладні відомості див. в статті [Визначення правила передавання пошти для шифрування](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="8a694-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="8a694-106">У PowerShell скористайтеся командлетом [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) і задайте значення "$true" для параметра *ApplyOME*.</span><span class="sxs-lookup"><span data-stu-id="8a694-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
