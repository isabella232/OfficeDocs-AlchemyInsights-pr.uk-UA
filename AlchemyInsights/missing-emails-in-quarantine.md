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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831755"
---
# <a name="missing-emails-in-quarantine"></a>Повідомлення електронної пошти відсутні в карантинах

Адміністратори можуть [переглядати, випускати та видаляти ці повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Щоб відкрити Центр безпеки &, перейдіть [https://protection.office.com](https://protection.office.com/) до . Щоб відкрити сторінку безпосередньо в карантин, перейдіть на сторінку [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Ви можете шукати за такими значеннями:  

- **Ідентифікатор повідомлення:** глобальний унікальний ідентифікатор повідомлення. Якщо вибрати повідомлення в списку, в **області** Відомості,  що з'явиться, з'явиться значення Ідентифікатор повідомлення. Адміністратори можуть використовувати [трасування повідомлень,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) щоб знаходити повідомлення та відповідні значення ідентифікаторів повідомлень.
- **Адреса електронної пошти відправника:** адреса електронної пошти одного відправника.
- **Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.
- **Тема**– використовуйте всю тему повідомлення. У результатах пошуку не врагується регістр.

Ввівши умови пошуку, натисніть кнопку Оновити, щоб ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **відфільтрувати** результати.  

Командлети, які використовуються для перегляду повідомлень і файлів і керування ними в карантині:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)зверніть увагу, що цей командлет призначено лише для повідомлень, які не призначено для зловмисних програм, які не підтримуються у службах SharePoint Online, "OneDrive для бізнесу" та Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)