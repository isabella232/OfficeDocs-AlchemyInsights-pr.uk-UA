---
title: Захист від атаки Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037183"
---
# <a name="protection-from-backscatter-attack"></a>Захист від атаки Backscatter

Backscatter – це звіти про недоставку (також відомі як NDRs або Bounce повідомлення), які ви отримали для повідомлень, які не надсилали. Спамери Forge (пародія) **від:** адреса своїх повідомлень, і вони часто використовують реальні адреси електронної пошти, щоб надати довіру до своїх повідомлень. Таким чином, коли спамери неминуче надсилають повідомлення неіснуючим одержувачам, поштовий сервер призначення суттєво обманом повертає повідомлення, що не вдалося знайти в повідомленні про НЕДОСТАВКУ, до кованого відправника в адресі **From:** Address (адреса).

Додаткові відомості можна знайти в [Backscatter в EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Увімкнення захисту від Backscatter**

Щоб увімкнути захист Backscatter, виконайте наведені нижче вказівки.

**protection.office.com > керування загрозою > політики > антиспам > виберіть політику фільтра спаму та редагувати політику > спам-властивості > позначки як спам > НЕДОСТАВКУ Backscatter > установіть його на "увімкнуто"**

Якщо ви вважаєте, що обліковий запис було скомпрометовано, ознайомтеся з такими:

- [Відповідь на несанкціонований обліковий запис електронної пошти](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Видалення заблокованих користувачів із порталу обмеженого користувача в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



