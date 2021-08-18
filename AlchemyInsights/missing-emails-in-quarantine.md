---
title: Відсутні електронні листи в карантині
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329683"
---
# <a name="missing-emails-in-quarantine"></a>Відсутні електронні листи в карантині

Адміністратори можуть [переглядати, випускати та видаляти ці повідомлення](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

На порталі Microsoft 365 Defender <https://security.microsoft.com> перейдіть до в меню **Review** \> **Quarantine (Переглянути карантин).** Або, щоб перейти безпосередньо до сторінки **"Карантин",** <https://security.microsoft.com/quarantine> скористайтеся .  

Докладні відомості про значення пошуку та фільтрування див. в розділі Керування повідомленнями та файлами в карантині як адміністратор служби [EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Командлети, які використовуються для перегляду повідомлень і файлів у карантинах і керування ними:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)зверніть увагу, що цей командлет доступний лише для повідомлень, а не файлів із Сейф Вкладення для SharePoint, OneDrive або Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
