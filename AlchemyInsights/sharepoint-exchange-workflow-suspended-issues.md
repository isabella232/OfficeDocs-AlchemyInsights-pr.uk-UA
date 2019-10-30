---
title: Початок роботи з SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766912"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="cad33-102">Робочі цикли в SharePoint</span><span class="sxs-lookup"><span data-stu-id="cad33-102">Workflows in SharePoint</span></span>

<span data-ttu-id="cad33-103">Якщо SharePoint робочі цикли не надсилають повідомлення електронної пошти, можливо, ваша організація зіткнулася з меж відправника Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="cad33-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="cad33-104">Повідомлення про помилку "робочий процес призупинено" може виникнути, якщо один із таких елементів:</span><span class="sxs-lookup"><span data-stu-id="cad33-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="cad33-105">У вас є робочий цикл SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="cad33-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="cad33-106">Робочий цикл налаштовано на надсилання настроюваного повідомлення електронної пошти більш ніж 200 користувачів одночасно, більше 10 000 одержувачів на день або більше 30 повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="cad33-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="cad33-107">Під час запуску робочого циклу повідомлення електронної пошти не надіслано, і ви помітите повідомлення про помилку, внутрішній стан встановлено призупинено або не вдається надіслати одержувачу відображається.</span><span class="sxs-lookup"><span data-stu-id="cad33-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="cad33-108">Для отримання додаткової інформації, будь ласка, зверніться до наступній [статті](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="cad33-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

