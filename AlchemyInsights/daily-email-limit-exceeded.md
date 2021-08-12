---
title: Перевищено щоденне обмеження електронної пошти. Робочий цикл призупинено.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914672"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Перевищено щоденне обмеження електронної пошти. Робочий цикл призупинено.

Ця помилка може з'явитися в таких випадках:

- У вас є робочий цикл в SharePoint Online, який використовує тип платформи робочих SharePoint 2010 SharePoint 2013 року.
- Робочий цикл настроєно на надсилання настроюваного повідомлення електронної пошти понад 200 користувачів за раз, понад 10 000 одержувачів на день або понад 30 повідомлень за хвилину.
- Під час запуску робочого циклу повідомлення електронної пошти не надсилається, і ви помітите таке:
    - Якщо робочий цикл використовується SharePoint 2013 року, потрібно перейти на сторінку **"Стан робочого циклу".** На сторінці "Стан робочого циклу" для параметра **Внутрішній** стан установлено значення Запущено **,** а у виносці з інформацією відображається повідомлення Не вдалося надіслати **одержувачу**.

Щоб вирішити цю проблему, настройте робочий цикл так, щоб він надсилав повідомлення електронної пошти, не перевищивши [обмеження Exchange Online відправників.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Наприклад, використовуйте паузу в робочому циклі, надішліть повідомлення електронної пошти групі Microsoft 365, групі розсилки чи поштовій групі безпеки або надішліть повідомлення менше ніж 200 одержувачам одночасно.


Докладні відомості див. в цій [статті.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Пов’язані теми
- [Створення Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 