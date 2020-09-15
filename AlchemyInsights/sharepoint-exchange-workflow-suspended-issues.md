---
title: Початок роботи зі службою SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700728"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="82e55-102">Робочі цикли в SharePoint</span><span class="sxs-lookup"><span data-stu-id="82e55-102">Workflows in SharePoint</span></span>

<span data-ttu-id="82e55-103">Якщо робочі цикли SharePoint не надсилають повідомлення електронної пошти, можливо, ваша організація виявила обмеження відправника в службі Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="82e55-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="82e55-104">Повідомлення про помилку "робочий цикл призупинено" може виникати, якщо у вас є один із таких способів:</span><span class="sxs-lookup"><span data-stu-id="82e55-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="82e55-105">Ви маєте робочий цикл у службі SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="82e55-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="82e55-106">Робочий цикл настроєно для надсилання настроюваного повідомлення електронної пошти для більш ніж 200 користувачів за один раз, понад 10 000 одержувачів на день або понад 30 повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="82e55-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="82e55-107">Під час запуску робочого циклу повідомлення електронної пошти не надсилається, і ви помітите повідомлення про помилку, внутрішній стан має значення призупинено або не вдається надіслати одержувачу.</span><span class="sxs-lookup"><span data-stu-id="82e55-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="82e55-108">Щоб отримати докладніші відомості, ознайомтеся з наведеними нижче [статтею](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="82e55-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

