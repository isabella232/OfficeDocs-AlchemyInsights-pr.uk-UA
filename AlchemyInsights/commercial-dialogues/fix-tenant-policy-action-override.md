---
title: Виправлення політики клієнта (заміна дії)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896096"
---
# <a name="fix-tenant-policy-action-override"></a>Виправлення політики клієнта (заміна дії)

Це повідомлення вплинуло одна з політик захисту від спаму. Щоб переглянути політики, виконайте такі дії:

1. На порталі Microsoft 365 Defender у розділі Політики співпраці & електронної пошти & правила захисту від <https://security.microsoft.com/>  \>  \>  \>  спаму. 

   Щоб перейти безпосередньо на сторінку **політики захисту від спаму,** <https://security.microsoft.com/antispam> скористайтеся .

2. На сторінці **Політики** захисту від спаму виберіть політику, клацнувши ім'я політики  **(** Тип – Спеціальна політика захисту від спаму або Ім'я – Політика захисту від спаму **(за замовчуванням)**). 
3. В області відомостей, що з'явиться, у розділі Дії **виберіть** **Редагувати** дії.
4. У розділі Дії з **повідомленнями** перегляньте вирази для **спаму,** високої достовірності спаму,  **фішинг** і Висока довірча фішинг, щоб перевірити, чи вибрано будь-яке з таких значень: 
   - **Додавання верхнього колонтитула X**
   - **Додавання тексту перед рядком теми**
   - **Переспрямування повідомлення на адресу електронної пошти**
   - **Видалення повідомлення**
   - **Жодних дій**

   Можливо, що повідомлення **вплинули** на Exchange Online Protection стандартні параметри.

Докладні відомості див. в ційи: Настроювання політик захисту [від спаму в EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
