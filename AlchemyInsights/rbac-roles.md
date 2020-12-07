---
title: 'Ролі RBAC '
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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583957"
---
# <a name="rbac-rules"></a>Правила RBAC

Якщо з'являється повідомлення про помилку з дозволом: 

- **Клієнт із ідентифікатором об'єкта не має дозволу на виконання дій над областю (код: не вдалося знайти)**: під час спроби створити ресурс переконайтеся, що ви ввійшли в обліковий запис користувача, якому призначено роль, яка має право на записування до ресурсу в вибраній області. Наприклад, щоб керувати віртуальними машинами у групі ресурсів, необхідно мати роль [учасника віртуальної машини](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в групі ресурсів (або батьківській області). Список дозволів для кожної вбудованої ролі наведено [в статті вбудовані ролі для ресурсів Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- У **вас немає дозволу на створення запиту на підтримку**: під час спроби створити або оновити квиток служби підтримки переконайтеся, що ви зараз ввійшли в обліковий запис, який має роль Microsoft. підтримка/supportTickets/Write, як-от [вкладник "запит на підтримку](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)".
- **Не можна створити більше призначень ролей (код: RoleAssignmentLimitExceeded)**: під час спроби призначити роль спробуйте зменшити кількість призначень ролей, призначаючи ролі до груп замість цього. Azure підтримує до завдань **2000** роль за передплатою.

Докладні відомості про ролі Блакитної RBAC наведено в статті [ролі БЛАКИТНОЇ RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
