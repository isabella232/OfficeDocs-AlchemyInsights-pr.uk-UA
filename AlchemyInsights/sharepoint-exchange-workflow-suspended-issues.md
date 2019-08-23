---
title: Початок роботи з SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: ae27a9fc342eb4fc4633ffd5518d63600b978db8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504016"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="3de86-102">Робочі процеси в SharePoint</span><span class="sxs-lookup"><span data-stu-id="3de86-102">Workflows in SharePoint</span></span>

<span data-ttu-id="3de86-103">Якщо робочі процеси SharePoint не відправляти електронну пошту, ваша організація можливо, зіткнулися Exchange Online межі відправника.</span><span class="sxs-lookup"><span data-stu-id="3de86-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="3de86-104">'Призупиняється робочий процес' повідомлення про помилку може виникнути, якщо у вас один з наступних пунктів:</span><span class="sxs-lookup"><span data-stu-id="3de86-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="3de86-105">У вас робочий процес у SharePoint Online, що використовує SharePoint 2010 або тип платформи робочого циклу SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="3de86-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="3de86-106">Робочий процес настроєний на надсилання повідомлення електронної пошти користувача більш ніж 200 користувачам час, більш ніж 10000 одержувачів на день або більше 30 повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="3de86-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="3de86-107">Якщо запустити робочий процес, не буде надіслано повідомлення електронної пошти і ви помітили помилку, слід установити внутрішній стан відображається перерване або не вдалося надіслати одержувачу.</span><span class="sxs-lookup"><span data-stu-id="3de86-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="3de86-108">Для отримання додаткової інформації будь ласка, зверніться до такої [статті](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="3de86-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

