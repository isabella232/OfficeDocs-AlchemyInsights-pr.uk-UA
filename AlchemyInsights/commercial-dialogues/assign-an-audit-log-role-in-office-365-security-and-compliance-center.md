---
title: Призначення ролі журналу аудиту в центрі відповідності системи безпеки Office 365 &
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749527"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Призначення ролі журналу аудиту в центрі відповідності системи безпеки Office 365 &

Щоб виконати пошук у журналі аудиту Office 365, адміністратор має призначати роль **журналів аудиту лише для перегляду** або роль **журналів аудиту** в службі Exchange Online. Ці ролі призначено для керування відповідністю і групами ролей керування організацією за замовчуванням. Глобальні адміністратори в Office 365 і Microsoft 365 автоматично додаються як учасники групи ролей керування організацією.

Щоб дозволити користувачу виконувати пошук за мінімальним рівнем привілеїв, створіть настроювану рольову групу в службі Exchange Online, **додайте роль** журналів аудиту, що стосується **лише подання** , а потім додайте користувача як учасника нової рольової групи.

Докладні відомості наведено в статті [Керування рольовими групами в службі Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) і [Пошук у журналі аудиту в центрі відповідності безпеки &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).