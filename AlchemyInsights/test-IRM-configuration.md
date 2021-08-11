---
title: Перевірка конфігурації IRM для нових можливостей OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812450"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Перевірка конфігурації IRM для нових можливостей OME

Щоб переконатися, що ваш Microsoft 365 настроєний на використання нових можливостей OME, запустіть наведені нижче командлети під час підключення [Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Перевірте конфігурацію IRM свого клієнта, запустивши `Get-IRMConfiguration` . Переконайтеся, що для цих значень установлено **значення True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Використовуючи свій домен, адресу відправника й одержувача, запустіть `Test-IRMConfiguration` . Якщо перевірка не пройде перевірку, перевірте конфігурацію IRM.

Докладні відомості про те, як перевірити конфігурацію IRM, див. в статті Перевірка нової конфігурації OME в [Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)