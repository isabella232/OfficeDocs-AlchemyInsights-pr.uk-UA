---
title: 'РОЛІ RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923152"
---
# <a name="rbac-rules"></a>Правила RBAC

Якщо з'являється повідомлення про помилку дозволів: 

- Клієнт із ідентифікатором об'єкта не має дозволу на виконання дій за областю **(код: AuthorizationFailed):** коли ви намагаєтеся створити ресурс, переконайтеся, що ви ввійшли під обліковим записом користувача з роллю, який має дозвіл на записування ресурсу у вибраній області. Наприклад, щоб керувати віртуальними машинами в групі [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) ресурсів, потрібно мати роль "Учасник віртуального комп'ютера" в групі ресурсів (або батьківській області). Список дозволів для кожної вбудованої ролі див. в розділі [Вбудовані ролі для ресурсів Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- У вас немає дозволу на створення запиту на **підтримку.** Під час спроби створити або оновити запит на підтримку переконайтеся, що ви ввійшли під обліковим записом користувача, чи призначено роль, яка має дозвіл Microsoft.Support/supportTickets/write, наприклад [Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)для запитів на підтримку.
- Більше не можна створювати призначення ролей **(код: RoleAssignmentLimitExceed).** Коли ви намагаєтеся призначити роль, спробуйте зменшити кількість призначень ролей, призначивши натомість ролі групам. Azure підтримує до **2000 призначень** ролей для передплати.

Докладні відомості про ролі Azure RBAC див. в [ролях Azure RBAC.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
