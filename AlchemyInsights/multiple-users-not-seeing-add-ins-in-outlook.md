---
title: Кілька користувачів, які не бачать надбудови, у програмі Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198246"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="00eb6-102">Кілька користувачів, які не бачать надбудови, у програмі Outlook</span><span class="sxs-lookup"><span data-stu-id="00eb6-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="00eb6-103">Якщо перевірити Outlook надбудови і не відображаються, як перший крок для виправлення неполадок, використовуйте командлет **Get-Організаціїconfig** PowerShell запит _Appsforofficeenabled_ параметр.</span><span class="sxs-lookup"><span data-stu-id="00eb6-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="00eb6-104">Якщо запит повертає значення **false**, установіть цей параметр **True** за допомогою командлета **Set-організаціїconfig** , тому надбудови відображаються належним чином.</span><span class="sxs-lookup"><span data-stu-id="00eb6-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="00eb6-105">Ми не рекомендуємо, що _Appsforofficeenabled_ параметр значення **false**.</span><span class="sxs-lookup"><span data-stu-id="00eb6-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="00eb6-106">Значення **false** скасовує всі вищевикладені адміністративні та настройки ролей користувача і запобігає активації будь-якого користувача в організації будь-які нові програми.</span><span class="sxs-lookup"><span data-stu-id="00eb6-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="00eb6-107">Для отримання додаткових відомостей див. [зазначення адміністраторів і користувачів, які можуть інсталювати надбудови Outlook і керувати ними](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="00eb6-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>