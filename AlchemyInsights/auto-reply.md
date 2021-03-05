---
title: 'Щоб настроїти автоматичну відповідь для всіх повідомлень електронної пошти, надісланих до групи Microsoft 365:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482890"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a><span data-ttu-id="7c994-102">Щоб настроїти автоматичну відповідь для всіх повідомлень електронної пошти, надісланих до групи Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7c994-102">To configure auto reply for all emails sent to Microsoft 365 group:</span></span>

<span data-ttu-id="7c994-103">**Підключіться до EXO PowerShell за допомогою облікового запису адміністратора клієнта та виконайте таку команду**:</span><span class="sxs-lookup"><span data-stu-id="7c994-103">**Connect to EXO PowerShell using tenant admin account and use following command**:</span></span>

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> <span data-ttu-id="7c994-104">Щоб змінити ім'я групи, на якому потрібно настроїти автоматичну відповідь **, змініть її** .</span><span class="sxs-lookup"><span data-stu-id="7c994-104">Change **groupmailbox** to a group name that you want to configure auto reply on.</span></span>

