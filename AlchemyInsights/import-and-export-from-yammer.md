---
title: Імпорт і експорт з Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037254"
---
# <a name="import-and-export-from-yammer"></a>Імпорт і експорт з Yammer

**Імпорт**

Варіанти імпорту користувача залежать від того, чи мережа Yammer працює в [рідному режимі для Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)або ні.

- **Нерідний режим**: користувачі можуть імпортувати їх до груп за допомогою [Додавання з адресної книги](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (обмеження до 100 користувачів) в межах групи або в мережі за допомогою [групового оновлення](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) в межах мережі.
- **Рідний режим**: операції з членством у групах і членство в мережі мають виконуватися на [порталі адміністрування Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), порталу " [Лазурний](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)" або за допомогою іншого параметра Azure AD. Мережі в рідному режимі більше не мають доступу до групового оновлення та інших застарілих функцій.

> [!IMPORTANT]
> Yammer ніколи не підтримував імпорт вмісту з адміністратора мережі, навіть коли в іншій мережі використовувався функція експорту даних. Вміст може бути повторно надіслано партнерськими рішеннями або API REST Yammer.

**Експорт**

[Експорт даних мережі в межах адміністратора мережі](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) дає можливість експортувати вміст у мережі Yammer, зокрема про повідомлення та файли. Вкладення можуть бути надзвичайно великими, і це призведе до того, що експорт матиме значний час для виконання. Ми рекомендуємо активувати активні мережі за допомогою [API експорту даних](https://developer.yammer.com/docs/data-export-api) на шматки за день або тиждень. Служба підтримки Microsoft не надає спеціальні сценарії для цієї мети.

Для експорту вмісту для окремого користувача існує окремий [експорт Гдпр](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) .