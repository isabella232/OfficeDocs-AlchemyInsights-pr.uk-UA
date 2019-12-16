---
title: Перевищено граничну кількість щоденних повідомлень електронної пошти. Робочий процес призупинено.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053138"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Перевищено граничну кількість щоденних повідомлень електронної пошти. Робочий процес призупинено.

Цю помилку можна отримати у таких випадках:

- У вас є робочий цикл SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.
- Робочий цикл налаштовано на надсилання настроюваного повідомлення електронної пошти більш ніж 200 користувачів одночасно, більше 10 000 одержувачів на день або більше 30 повідомлень за хвилину.
- Під час запуску робочого циклу, повідомлення електронної пошти не надіслано, і ви помітите, що така поведінка:
    - Для робочого циклу, використовуючи тип платформи SharePoint 2013, перейдіть на сторінку **стан робочого циклу** . На сторінці стан робочого циклу **внутрішній стан** налаштовано на **початок**, а інформаційна виноска **не може надіслати одержувачу**.

Щоб вирішити цю проблему, настройте робочий цикл для надсилання повідомлень електронної пошти без перевищення [меж відправника Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Наприклад, використовуйте паузу в робочому циклі, надішліть повідомлення електронної пошти на групу Office 365, групу розсилки або поштову групу безпеки або надішліть повідомлення менше ніж 200 одержувачам одночасно.


Щоб отримати додаткові відомості, зверніться до такої [статті](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Пов’язані теми
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 