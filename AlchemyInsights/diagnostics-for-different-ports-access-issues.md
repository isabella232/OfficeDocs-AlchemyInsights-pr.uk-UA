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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="acbfd-102">Діагностика для різних проблем із доступом до портів</span><span class="sxs-lookup"><span data-stu-id="acbfd-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="acbfd-103">Щоб вирішити різні проблеми з доступом до портів, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="acbfd-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="acbfd-104">Зупиніть або девиділяє віртуальну машину (VM) на порталі, перезавантажте VM та повторіть спробу.</span><span class="sxs-lookup"><span data-stu-id="acbfd-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="acbfd-105">Перевірте параметри мережі ВМ, щоб визначити, чи є у вас групи безпеки мережі (NSGs), що блокує трафік.</span><span class="sxs-lookup"><span data-stu-id="acbfd-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="acbfd-106">Ви також можете використовувати [IP-потік мережі Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , щоб перевірити, чи не блокує трафік, User-Defined маршрутів (udrs), щоб повернути трафік до локального ("маршрут за замовчуванням" 0.0.0.0/0) або до мережевого пристрою.</span><span class="sxs-lookup"><span data-stu-id="acbfd-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="acbfd-107">Якщо після виконання наведених вище дій виникли проблеми, укажіть ім'я ВМ та TCP-порт, на який ви намагаєтеся надіслати пошту, щоб продовжити діагностику.</span><span class="sxs-lookup"><span data-stu-id="acbfd-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="acbfd-108">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="acbfd-108">**Recommended Documents**</span></span>

[<span data-ttu-id="acbfd-109">Обмеження та рекомендації щодо надсилання вихідної пошти через порт 25</span><span class="sxs-lookup"><span data-stu-id="acbfd-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)