---
title: Діагностика для різних проблем із доступом до портів
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036804"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Діагностика для різних проблем із доступом до портів

Щоб вирішити різні проблеми з доступом до портів, виконайте наведені нижче дії.

1. Зупиніть або девиділяє віртуальну машину (VM) на порталі, перезавантажте VM та повторіть спробу. 
2. Перевірте параметри мережі ВМ, щоб визначити, чи є у вас групи безпеки мережі (NSGs), що блокує трафік. Ви також можете використовувати [IP-потік мережі Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , щоб перевірити, чи не блокує трафік, User-Defined маршрутів (udrs), щоб повернути трафік до локального ("маршрут за замовчуванням" 0.0.0.0/0) або до мережевого пристрою.
Якщо після виконання наведених вище дій виникли проблеми, укажіть ім'я ВМ та TCP-порт, на який ви намагаєтеся надіслати пошту, щоб продовжити діагностику.

**Рекомендовані документи**

[Обмеження та рекомендації щодо надсилання вихідної пошти через порт 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)