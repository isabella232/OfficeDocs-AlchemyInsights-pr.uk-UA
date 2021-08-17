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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892068"
---
# <a name="missing-emails-in-quarantine"></a>Відсутні електронні листи в карантині

Адміністратори можуть [переглядати, випускати та видаляти ці повідомлення](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

На порталі Microsoft 365 Defender перейдіть <https://security.microsoft.com> до меню **Перегляд** \> **карантин.** Або, щоб перейти безпосередньо до сторінки **"Карантин",** <https://security.microsoft.com/quarantine> скористайтеся .  

Докладні відомості про значення пошуку та фільтрування див. в розділі Керування повідомленнями та файлами в карантині як адміністратор служби [EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Командлети, які використовуються для перегляду повідомлень і файлів у карантинах і керування ними:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)зверніть увагу, що цей командлет доступний лише для повідомлень, а не файлів із Сейф Вкладень для SharePoint, OneDrive або Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
