---
title: Поняття розширеної автентифікації, які Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934386"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Поняття розширеної автентифікації, які Microsoft Edge

Нижче наведено поняття розширеної автентифікації, які застосовуються до Microsoft Edge.

**Proactive Authentication**

Якщо ввімкнути політику [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge спробує завбачливо автентифікувати користувачів, які ввійшли в службу, служби Microsoft. Через регулярні проміжки часу вона використовуватиме онлайнову службу, щоб перевіряти наявність оновлених маніфестів, які містять конфігурацію, що регулює proactive Authentication (Проактивна автентифікація).

Переваги. Завбачлива автентифікація активує автентифікацію для ключових служб, наприклад Office сторінки нової вкладки. Крім того, якщо Bing використовується як пошуковий запит, Proactive Authentication покращує продуктивність рядка адреси та допомагає генерувати результати пошуку, персоналізовані за потреби компанії.

**Windows Hello CredUI для автентифікації NTLM**

Якщо єдиний вхід (SSO) недоступний, якщо веб-сайт намагається ввійти в користувача через механізм NTLM або переговорів, ця функція дасть змогу користувачу надати веб-сайту спільний доступ до облікових даних ОС і задовольнити проблему з автентифікацією за допомогою інтерфейсу користувача Windows Hello Cred. Цей процес входу відображатиметься лише в Windows 10 лише для користувачів, які не отримують єдиного входу під час NTLM або домовленості.

**Використання збережених паролів для автоматичного входу**

Користувачі, які зберігають паролі в Microsoft Edge можуть активувати автоматичний вхід на веб-сайти, на яких збережено облікові дані. Користувачі можуть увімкнути або вимкнути цю функцію в edge://settings/passwords, а також налаштувати її в [політиках диспетчера паролів.](https://go.microsoft.com/fwlink/?linkid=2134622)
