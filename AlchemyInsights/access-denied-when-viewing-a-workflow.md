---
title: Відмовлено в доступі під час перегляду робочого процесу
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050546"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="175c3-102">Відмовлено в доступі під час перегляду робочого процесу</span><span class="sxs-lookup"><span data-stu-id="175c3-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="175c3-103">SharePoint 2013 робочих циклів, які намагаються надіслати повідомлення електронної пошти до групи SharePoint може не з повідомлення про помилку "немає доступу", якщо членство групи SharePoint не встановлено для всіх.</span><span class="sxs-lookup"><span data-stu-id="175c3-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="175c3-104">**Щоб вирішити цю проблему, виконайте такі дії:**</span><span class="sxs-lookup"><span data-stu-id="175c3-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="175c3-105">Дозволити всім користувачам бачити учасників групи SharePoint.</span><span class="sxs-lookup"><span data-stu-id="175c3-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="175c3-106">Видалити групу SharePoint, з до або копія рядок повідомлення електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="175c3-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="175c3-107">Явно додати користувачів до рядка кому або копія, якщо видимість членства не можна змінити для групи SharePoint.</span><span class="sxs-lookup"><span data-stu-id="175c3-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="175c3-108">Для перегляду більш детальної інформації, будь ласка, зверніться до [http несанкціонованого доступу до/_vti_bin/Client.SVC/SP.utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="175c3-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  