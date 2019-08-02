---
title: Email Ліміт добової перевищено. Робочий процес буде призупинено.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059659"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Щоденне електронне повідомлення вичерпана. Робочий процес буде призупинено.

Ця помилка може бути отримана в таких випадках:

- У вас робочий процес у SharePoint Online, що використовує SharePoint 2010 або тип платформи робочого циклу SharePoint 2013.
- Робочий процес настроєний на надсилання повідомлення електронної пошти користувача більш ніж 200 користувачам час, більш ніж 10000 одержувачів на день або більше 30 повідомлень за хвилину.
- Під час запуску робочого процесу, не буде надіслано сповіщення електронною поштою, а ви помітили, що така поведінка:
    - Для робочого процесу за допомогою SharePoint 2013 тип платформи ви перейдіть до сторінки **Стану робочого процесу** . На сторінці стану робочих **Started**встановлено **Внутрішній світ** і повітряна куля інформації відображає **не вдалося надіслати одержувачу**.

Щоб вирішити цю проблему, настройте робочий процес надсилання повідомлень електронної пошти без перевищення [Exchange Online відправника меж](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Наприклад, використовуйте пауза робочого циклу, надіслати електронну пошту до Office 365 Група, групу розсилки або групу безпеки пошти ввімкнуто або відправити повідомлення до менше ніж 200 одержувачів одночасно.


Докладніше перегляньте наступні [статті](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Пов’язані теми
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і потік](https://flow.microsoft.com/blog/sharepoint-and-flow/) 