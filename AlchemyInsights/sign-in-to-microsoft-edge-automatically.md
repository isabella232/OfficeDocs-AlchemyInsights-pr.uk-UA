---
title: Автоматичний вхід Microsoft Edge входу
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050715"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Автоматичний вхід Microsoft Edge входу

Microsoft Edge використовує стандартний обліковий запис ОС, щоб автоматично входити в обліковий запис користувача відповідно до настройок пристрою користувача. 

Нижче описано сценарії конфігурації кожного типу пристрою та залежні від користувача процедури входу.

- **Пристрій гібридний/AAD-J:** цей параметр доступний у Windows 10, на рівні Windows і у відповідних версіях сервера. Користувачі автоматично ввійшли за допомогою своїх облікових Azure Active Directory (AD).
- **Пристрій приєднано до** домену: цей параметр доступний на Windows 10, на рівні Windows та у відповідних версіях сервера. За замовчуванням користувачі з обліковими записами домену не ввійшли автоматично. щоб увімкнути автоматичний вхід до них, скористайтеся політикою **ConfigureOnPremisesAccountAutoSignIn.** Щоб активувати автоматичний вхід для користувачів з обліковими записами Azure AD, реоюендуйте гібридне приєднання до своїх пристроїв.
- Обліковий запис **Microsoft** за замовчуванням використовується в ос Windows 10 RS3 (версія 1709, збірка 10.0.16299) і новіших версіях. Навпаки, цей сценарій має трапитися на корпоративних пристроях. Однак, якщо за замовчуванням використовується обліковий запис Microsoft для ОС, Microsoft Edge автоматично ввійти в обліковий запис Microsoft.
 
 
