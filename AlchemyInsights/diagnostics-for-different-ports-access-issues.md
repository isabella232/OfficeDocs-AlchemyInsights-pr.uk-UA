---
title: Діагностика різних проблем із доступом до портів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030923"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Діагностика різних проблем із доступом до портів

Щоб усунути різні проблеми з доступом до порту, виконайте такі дії:

1. Зупиніть або угоди на віртуальній машині (VM) з порталу, перезапустіть віртуальну машину та перевірте ще раз. 
2. Перевірте параметри мережі VM, щоб з'ясувати, чи заблоковано трафік груп безпеки мережі (NSGs). Також за [](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) допомогою засобу перевірки IP-потоку мережевого стеження можна перевірити наявність NSG-файлів, які блокують трафік, маршрутизацію маршрутів User-Defined (UDRs) і перенаправляйте трафік до локального середовища ("Маршрут за замовчуванням" 0.0.0.0/0) або мережевому пристрої.
Якщо після описаних вище кроків проблеми не зникли, укажіть ім'я VM та порт TCP, на який ви намагаєтеся надіслати повідомлення для подальшого діагностики.

**Рекомендовані документи**

[Обмеження та рекомендації щодо надсилання вихідної електронної пошти через порт 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)