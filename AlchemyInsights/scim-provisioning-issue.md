---
title: Проблема підготовки SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949952"
---
# <a name="scim-provisioning-issue"></a>Проблема підготовки SCIM

Функція автоматичного підготовки відповідає за створення посвідчень та ролей користувачів у хмарних програмах, до яких користувачам потрібен доступ. Крім створення посвідчень користувачів, функція автоматичного підготовки включає в себе обслуговування та видалення посвідчень користувачів як зміни стану або ролей. Перш ніж почати розгортання, можна переглянути, [як працює підготовка](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) , щоб дізнатися, як працює положення Azure Active Directory (AD), а також отримати рекомендації з конфігурації.

Як розробник програми, ви можете використовувати систему для керування обліковими записами для перехресного домену (SCIM), щоб активувати автоматичну підготовку користувачів і груп між вашою програмою та Лазуровою ОБ'ЯВАМИ. У статті [створення кінцевої точки SCIM і настроювання підготовки користувачів за допомогою служби AZURE AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) . описується, як створити кінцеву точку SCIM і інтегрувати її в службу підготовки Azure AD.



