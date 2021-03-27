---
title: Поняття розширеної автентифікації, що застосовуються до Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398606"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Поняття розширеної автентифікації, що застосовуються до Microsoft Edge

Нижче наведено поняття розширеної автентифікації, які застосовуються до Microsoft Edge.

**Proactive Authentication**

Якщо ввімкнути політику [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge спробує завибачливо автентифікувати користувачів, які ввійшли в службу Microsoft. Через регулярні проміжки часу вона використовуватиме онлайнову службу, щоб перевіряти наявність оновлених маніфестів, які містять конфігурацію, що регулює proactive Authentication (Проактивна автентифікація).

Переваги. Завбачлива автентифікація активує автентифікацію для ключових служб, таких як сторінка Office New Tab Page (Нова вкладка Office). Крім того, якщо Bing використовується як пошуковий система, Proactive Authentication покращує продуктивність рядка адреси та допомагає генерувати результати пошуку, персоналізовані за потреби компанії.

**Автентифікація Windows Hello CredUI для автентифікації NTLM**

Якщо єдиний вхід (SSO) недоступний, якщо веб-сайт намагається ввійти в користувача через механізм NTLM або вести переговори, ця функція дасть змогу користувачу надати доступ до облікових даних ОС із веб-сайту та задовольнити проблему автентифікації за допомогою інтерфейсу користувача Windows Hello Cred. Цей процес входу відображатиметься лише у Windows 10 і лише для користувачів, які не отримують єдиного входу під час NTLM або домовленості.

**Використання збережених паролів для автоматичного входу**

Користувачі, які зберігають паролі в Microsoft Edge, можуть активувати автоматичний вхід на веб-сайти, на яких збережено облікові дані. Користувачі можуть увімкнути або вимкнути цю функцію в edge://settings/passwords, а також налаштувати її в [політиках диспетчера паролів.](https://go.microsoft.com/fwlink/?linkid=2134622)
