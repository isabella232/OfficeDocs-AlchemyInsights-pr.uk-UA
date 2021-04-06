---
title: Засіб діагностики служби для віртуального робочого стола Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596043"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Засіб діагностики служби для віртуального робочого стола Windows

Віртуальний робочий стіл Windows (WVD) пропонує засіб діагностики, який дає змогу адміністраторам визначити помилки в одному інтерфейсі. Цей засіб реєструє діагностичні відомості щоразу, коли WVD використовується користувачем, який призначає роль WVD. Кожен журнал містить відомості про роль WVD, залучену до дії, повідомлення про помилку, які відображаються під час сеансу, а також відомості про клієнта та користувача. Аналітика журналів Azure можна налаштувати на записування журналу дій, створеного засобом діагностики, виконавши такі дії:

1. Створіть робочу область Log Analytics за допомогою [порталу Azure](https://go.microsoft.com/fwlink/?linkid=2129500) або [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Підключіть комп'ютери з Windows до монітора Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Отримайте ідентифікатор робочої області та первинний ключ робочої області. Ці відомості необхідно налаштувати в майстрі налаштування для належного налаштування агента та забезпечення його зв'язку з монітором Azure.

1. [Push-дані діагностики до робочої області.](https://go.microsoft.com/fwlink/?linkid=2128284) Ви можете переносити діагностичні дані з клієнта WVD до аналітики журналів для робочої області.

1. [Визначте та діагностувати](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) проблеми, які є внутрішніми або зовнішніми у зв'язанні із WVD.

Докладні відомості про настроювання засобу діагностики служби для WVD див. в статтях Використання аналітики журналу для функції діагностики.