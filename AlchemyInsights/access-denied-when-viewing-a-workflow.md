---
title: Під час перегляду робочого циклу відмовлено в доступі
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688823"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="302fb-102">Під час перегляду робочого циклу відмовлено в доступі</span><span class="sxs-lookup"><span data-stu-id="302fb-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="302fb-103">Робочі цикли SharePoint 2013, які намагаються надіслати повідомлення електронної пошти до групи SharePoint, можуть не працювати з повідомленням про помилку "відмовлено в доступі", якщо членство в групі SharePoint не настроєно для всіх користувачів.</span><span class="sxs-lookup"><span data-stu-id="302fb-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="302fb-104">**Щоб вирішити цю проблему, виконайте наведені нижче дії.**</span><span class="sxs-lookup"><span data-stu-id="302fb-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="302fb-105">Дозволити всім користувачам бачити учасників групи SharePoint.</span><span class="sxs-lookup"><span data-stu-id="302fb-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="302fb-106">Видаліть групу SharePoint із рядка "Кому" або "Копія" повідомлення електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="302fb-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="302fb-107">Явно додати користувачів до рядка "Кому" або "Копія", якщо видимість членства не можна змінити для групи SharePoint.</span><span class="sxs-lookup"><span data-stu-id="302fb-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="302fb-108">Щоб переглянути докладні відомості, зверніться до [http-неавторизованого доступу до/_vti_bin/Client.SVC/SP.utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="302fb-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  