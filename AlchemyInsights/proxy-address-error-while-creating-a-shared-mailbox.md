---
title: Помилка адреси проксі-сервера під час створення спільної поштової скриньки
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568311"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="8ef68-102">Помилка адреси проксі-сервера під час створення поштової скриньки або іншого об'єкта з увімкнутим повідомленням електронної пошти</span><span class="sxs-lookup"><span data-stu-id="8ef68-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="8ef68-103">Якщо ви спробували створити об'єкт із підтримкою електронної пошти (поштова скринька, Спільна поштова скринька тощо), і отримано повідомлення про помилку "Адреса проксі-сервера" SMTP:alias@domain.com "уже використовується...", вибрана адреса електронної пошти вже береться за допомогою іншого об'єкта, який підтримує електронну пошту, у вашій організації.</span><span class="sxs-lookup"><span data-stu-id="8ef68-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="8ef68-104">Потрібно відшукати користувача, групу, спільну поштову скриньку або спільну папку з цією адресою електронної пошти та видалити його або змінити її адресу електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="8ef68-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="8ef68-105">Потім можна створити новий об'єкт із підтримкою електронної пошти з звільненою адресою електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="8ef68-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="8ef68-106">Скористайтеся пошуком на головній сторінці, щоб знайти його.</span><span class="sxs-lookup"><span data-stu-id="8ef68-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="8ef68-107">Щоб знайти його, можна також скористатися наведена нижче командою Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8ef68-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="8ef68-108">Якщо ви не хочете видаляти наявну адресу електронної пошти, виберіть нову адресу електронної пошти для нового об'єкта, який ви створюєте.</span><span class="sxs-lookup"><span data-stu-id="8ef68-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  