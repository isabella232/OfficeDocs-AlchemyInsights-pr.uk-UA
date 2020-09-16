---
title: Перевищено граничний обсяг щоденного повідомлення електронної пошти. Робочий цикл призупинено.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731584"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Перевищено граничний обсяг щоденного повідомлення електронної пошти. Робочий цикл призупинено.

Цю помилку можна отримати в таких ситуаціях:

- Ви маєте робочий цикл у службі SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.
- Робочий цикл настроєно для надсилання настроюваного повідомлення електронної пошти для більш ніж 200 користувачів за один раз, понад 10 000 одержувачів на день або понад 30 повідомлень за хвилину.
- Під час запуску робочого циклу повідомлення електронної пошти не надсилається, і ви помітите таку поведінку:
    - Для робочого циклу за допомогою типу платформи SharePoint 2013 можна перейти на сторінку " **стан робочого циклу** ". На сторінці "стан робочого циклу" установлено **внутрішній стан** " **початок**", а повітряна кулька "відомості" **не може бути надіслано одержувачу**.

Щоб вирішити цю проблему, настройте робочий цикл, щоб надсилати повідомлення електронної пошти, не перевищивши [обмеження відправника Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Наприклад, за допомогою паузи в робочому циклі надішліть повідомлення електронної пошти до групи Microsoft 365, групі розсилки або з увімкнутою безпекою пошти або надішліть повідомлення менше, ніж 200 одержувачам за один раз.


Щоб отримати докладніші відомості, ознайомтеся з наведена нижче [статтею](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Пов’язані теми
- [Створення потоку](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і передавання](https://flow.microsoft.com/blog/sharepoint-and-flow/) 