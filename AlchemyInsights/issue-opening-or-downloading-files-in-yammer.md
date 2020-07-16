---
title: Проблеми з відкриттям або завантаженням файлів у Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148439"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Проблеми з відкриттям або завантаженням файлів у Yammer

Класична Yammer підтримує кілька варіантів завантаження файлів для повідомлень і груп. Залежно від конфігурації мережі, файли за замовчуванням для зберігання в SharePoint.

Вибір файлів у новій Yammer ще не підтримує всі параметри, доступні в класичній Yammer. Майбутні оновлення будуть додавати додаткові функції. Для отримання додаткових відомостей див. [додайте файл або зображення до повідомлення про розмову Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Не вдається відкрити або завантажити файл**  

Файл може бути вивантажене на Yammer, але також зв'язування з файлом у SharePoint Online. Щоб усунути неполадки, спочатку потрібно визначити розташування файлу. Якщо файл завантажено до Yammer, він матиме URL-адресу *. yammer.com. Переконайтеся, що потрібні URL-адреси та IP-адреси розблоковано. Для отримання додаткової інформації див у блозі [за допомогою жорстко кодованих IP-адрес для Yammer не рекомендується](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Перевірте, чи користувач, який також є глобальним адміністратором, може завантажити файл. Якщо файл приватний, можливо, доведеться використовувати режим приватного вмісту. Для отримання додаткових відомостей [див.](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)  

**Мережні гості та файли в SharePoint Online**  

[Мережні гості Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не ВИКОРИСТОВУЮТЬ AZURE AD B2B і є внутрішніми для служби Yammer, тому вони не можуть отримати доступ до файлів Yammer, збережених у SharePoint. Створення зовнішнього сад B2B користувача, який може отримати доступ до бібліотек документів SharePoint Online за допомогою цього посвідчення. Відомості про майбутні Azure AD B2B підтримки гостя в Yammer, зверніться [до служби підтримки користувачів бізнес-бізнесу (B2B), у вікні попереднього перегляду Yammer та FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).