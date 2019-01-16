---
title: Доступ заборонено під час перегляду робочого процесу
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318936"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d8f44-102">Доступ заборонено під час перегляду робочого процесу</span><span class="sxs-lookup"><span data-stu-id="d8f44-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d8f44-103">SharePoint 2013 робочі процеси, що спроба надіслати електронне повідомлення групі SharePoint може не спрацювати і повідомлення про помилку "Немає доступу" Якщо участь у групі SharePoint не розташований кожному.</span><span class="sxs-lookup"><span data-stu-id="d8f44-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d8f44-104">**Щоб вирішити цю проблему, виконайте такі дії:**</span><span class="sxs-lookup"><span data-stu-id="d8f44-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d8f44-105">Дозволити всім переглядати учасників групи SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8f44-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="d8f44-106">Видалення групи SharePoint із кому або копія лінія повідомлення електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="d8f44-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="d8f44-107">Явно додайте користувачів до кому або копія лінії, якщо для групи SharePoint не можна змінити членство видимість.</span><span class="sxs-lookup"><span data-stu-id="d8f44-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="d8f44-108">Для перегляду більш докладної інформації, будь ласка, зверніться до [HTTP-Unauthorized до /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d8f44-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

