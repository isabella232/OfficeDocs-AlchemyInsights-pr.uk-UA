---
title: Робочий робочий час для підготовки користувачів AD переходить у стан карантин
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036513"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Робочий робочий час для підготовки користувачів AD переходить у стан карантин

**Робочий робочий час для підготовки користувачів AD переходить у карантинний стан, і в ad не створюються жодні користувачі**

Завдання Workday to AD User Provisioning (Робочий день від AD до підготовчого користувача) перенесено в стан "карантин", а в контрольних журналах – події про помилку експорту з повідомленням про помилку **OperationsError-SvcErr: сталася помилка операції. Для служби каталогів не настроєно жодне покращене довідник. Таким чином, служба каталогів не може передати посилання на об'єкти за межами цього лісу.** Ця помилка зазвичай відображається, якщо OU контейнера Active Directory настроєно неправильно або виникають проблеми зіставленням виразів, що використовуються для **parentDistinguishedName.**

Переконайтеся, що для параметра New Users (Нові користувачі) за замовчуванням **вибрано** параметр OU. Переконайтеся, що вказаний оу вже існує в AD. Якщо в зіставленні атрибутів використовується **parentDistinguishedName,** переконайтеся, що вона завжди обчислена у відомому контейнері в домені AD. Перегляньте подію Export (Експорт) у контрольних журналах, щоб переглянути згенероване значення.

Докладні відомості про настроювання робочого робочого процесу для автоматичного підготовки див. в навчальній вправі: настроювання робочого місця для [автоматичного підготовки користувачів.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

