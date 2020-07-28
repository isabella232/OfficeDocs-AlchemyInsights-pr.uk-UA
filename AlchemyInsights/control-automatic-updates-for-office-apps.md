---
title: Керування автоматичними оновленнями для програм Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439929"
---
# <a name="control-automatic-updates-for-office-apps"></a>Керування автоматичними оновленнями для програм Office

За промовчанням оновлення для програм Office завантажуються автоматично та застосовуються у фоновому режимі без втручання користувача. Проте адміністратори можуть контролювати, як оновлення застосовуються за допомогою настройок служби Office Update. Параметри оновлення дають змогу адміністраторам вмикати й вимикати автоматичні оновлення, відображати або приховувати кнопку **оновити зараз** в Office, встановлювати терміни оновлення тощо. Докладні відомості див.:

- [Настроювання параметрів оновлення для Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Автоматичне оновлення для Office не ввімкнуто](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Визначення способу оновлення Office після інсталяції](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Щоб переглянути наявні настройки оновлень, застосовані до клієнтського комп'ютера, виконайте такі дії:

1. Відкрийте редактор **реєстру, перейшовши до запуску**  >  **Run**  >  **Regedit**.
2. Перейдіть до такого розташування та перегляньте параметри оновлення Office:  
    є. HKEY_LOCAL_MACHINE \ програмне Забезпечена\mice\офісr\  
    B. Параметри залипання кнопки миші

**Зверніть увагу**  Якщо встановлено ключ officemgmtcom, може відображатися повідомлення "оновлення керуються системним адміністратором **" у**оновлення Office для  >  **облікового запису**Office  >  **Office Updates**. Для отримання додаткових відомостей див. [керування оновленнями для microsoft 365 програм за допомогою диспетчера конфігурацій Microsoft кінцевої точки](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  