---
title: Автоматичний вхід у Microsoft Edge
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398750"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Автоматичний вхід у Microsoft Edge

Microsoft Edge використовує стандартний обліковий запис ОС, щоб автоматично входити в обліковий запис відповідно до настройок пристрою користувача. 

Нижче описано сценарії конфігурації кожного типу пристрою та залежні від користувача процедури входу.

- **Пристрій гібридний/AAD-J:** цей параметр доступний у Windows 10, нижче рівня Windows і у відповідних версіях сервера. Користувачі автоматично ввійшли за допомогою облікових записів Azure Active Directory (AD).
- **Пристрій приєднано до** домену: цей параметр доступний у Windows 10, на рівні нижче Windows і у відповідних версіях сервера. За замовчуванням користувачі з обліковими записами домену не ввійшли автоматично. щоб увімкнути автоматичний вхід до них, скористайтеся політикою **ConfigureOnPremisesAccountAutoSignIn.** Щоб активувати автоматичний вхід для користувачів з обліковими записами Azure AD, реоюендуйте гібридне приєднання до своїх пристроїв.
- Обліковий запис Microsoft за замовчуванням використовується в ОС **Windows** 10 RS3 (версія 1709, збірка 10.0.16299) і новіших версіях. Навпаки, цей сценарій має трапитися на корпоративних пристроях. Однак, якщо за замовчуванням використовується обліковий запис Microsoft для ОС, Microsoft Edge автоматично ввійме в обліковий запис Microsoft.
 
 
