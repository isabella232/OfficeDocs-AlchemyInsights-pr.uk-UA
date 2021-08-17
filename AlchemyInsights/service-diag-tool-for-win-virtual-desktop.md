---
title: Засіб діагностики служб Windows віртуальному робочому столі
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052407"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Засіб діагностики служб Windows віртуальному робочому столі

Windows Віртуальний робочий стіл (WVD) пропонує засіб діагностики, який дає адміністраторам змогу визначити помилки в одному інтерфейсі. Цей засіб реєструє діагностичні відомості щоразу, коли WVD використовується користувачем, який призначає роль WVD. Кожен журнал містить відомості про роль WVD, залучену до дії, повідомлення про помилку, які відображаються під час сеансу, а також відомості про клієнта та користувача. Аналітика журналів Azure можна настроїти так, щоб записувати журнал дій, створений засобом діагностики. Ось як це зробити.

1. Створіть робочу область Log Analytics за допомогою [порталу Azure](https://go.microsoft.com/fwlink/?linkid=2129500) або [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Підключення Windows'ютерів на монітор Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Отримайте ідентифікатор робочої області та первинний ключ робочої області. Ці відомості необхідно налаштувати в майстрі налаштування для належного налаштування агента та забезпечення його зв'язку з монітором Azure.
1. [Push-дані діагностики до робочої області.](https://go.microsoft.com/fwlink/?linkid=2128284) Ви можете переносити діагностичні дані з клієнта WVD до аналітики журналів для робочої області.
1. [Визначте та діагностувати](https://go.microsoft.com/fwlink/?linkid=2128338) проблеми, які є внутрішніми або зовнішніми у зв'язанні із WVD.

Докладні відомості про настроювання засобу діагностики служби для WVD див. в статтях Використання аналітики журналу для [функції діагностики.](https://go.microsoft.com/fwlink/?linkid=2128084)
