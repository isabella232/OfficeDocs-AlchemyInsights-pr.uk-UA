---
title: Розгортання надбудов для Програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125809"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Розгортання надбудов для Програми Microsoft 365

Централізоване розгортання – рекомендований спосіб розгортання Office надбудов для користувачів і груп в організації. Щоб розгорнути надбудови, виконайте наведені нижче дії.

**Примітка.** Відомості про інсталяцію надбудов Office як окремого користувача див. в статті Перегляд і інсталяція надбудов, а також керування [ними Office програмах.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Крім того, переконайтеся, що окреме придбання Office Надбудови з Магазину увімкнуто. 

1. Переконайтеся, що середовище відповідає вимогам до розгортання надбудов за допомогою централізованого розгортання. Докладніші відомості див. у [шкалику Вимоги](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Перейдіть до **Настройки**  >  **Інтегровані** програми Завантажити  >  **програми** Microsoft 365, щоб розгорнути надбудови. 

Примітки. 

- Щоб інтегрувати програми, адміністратор має дозволи глобального адміністратора Exchange адміністраторів.

- Розгортаючи надбудови для кількох користувачів, радимо робити завдання за допомогою груп, а не окремих користувачів. Докладні відомості див. в статтях Рекомендації щодо призначення [надбудови користувачам і групам.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Централізоване розгортання не підтримує користувачів у вкладених групах або групах, які мають батьківські групи. Докладні відомості [див. в цьому посібнику: призначення користувачів і груп.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Переконайтеся, що службу керування програмами Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') увімкнуто для користувачів для входу. Докладні відомості див. [в цьому вікні.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Якщо під час розгортання надбудов виникають проблеми з розгортанням за допомогою функції "Інтегровані програми", спробуйте розгорнути [їх за допомогою надбудов.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Докладні відомості:

[Розгортання надбудов у Центрі адміністрування](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Керування надбудовами в Центрі адміністрування](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 Керування надбудовами за допомогою командлетів [PowerShell централізованого розгортання](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Публікування Office надбудов за допомогою централізованого](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) розгортання в Центрі Microsoft 365 адміністрування 
 [Усунення несправностей: Користувач не бачить надбудови](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Виправлення помилок користувачів Office надбудовах](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)