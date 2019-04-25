---
title: Вирішення проблем із доставкою електронної пошти до пошти спільних папок
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401463"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="8cf1b-102">Вирішення проблем із доставкою електронної пошти до пошти спільних папок</span><span class="sxs-lookup"><span data-stu-id="8cf1b-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="8cf1b-103">Якщо зовнішніх відправників не вдається надіслати повідомлення до пошти спільних папок і відправників отримувати повідомлення про помилку: **не міг знайти (550 5.4.1)**, перевірити електронну пошту домену для спільних папок настроєно як внутрішній домен ретрансляції замість послугами авторитетний домен:</span><span class="sxs-lookup"><span data-stu-id="8cf1b-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="8cf1b-104">Відкрийте [Exchange admin центр (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="8cf1b-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="8cf1b-105">Перейдіть до **потоку пошти** \> **допустимих доменів**, виберіть допустимий домен і натисніть кнопку **редагувати**.</span><span class="sxs-lookup"><span data-stu-id="8cf1b-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="8cf1b-106">У властивості сторінки цього відкриється, якщо тип домену має значення **Authoritative**, змініть значення на **внутрішньої ретрансляції** і натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="8cf1b-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="8cf1b-107">Якщо зовнішніх відправників одержувати помилки, **ви не маєте дозволу (550 5.7.13)**, запустіть таку команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) бачити дозволи для анонімних користувачів у спільній папці:</span><span class="sxs-lookup"><span data-stu-id="8cf1b-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="8cf1b-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Наприклад, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="8cf1b-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="8cf1b-109">Щоб дозволити зовнішнім користувачам надсилати електронну пошту до цієї спільної папки, додати CreateItems доступу права користувача Анонім.</span><span class="sxs-lookup"><span data-stu-id="8cf1b-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="8cf1b-110">Наприклад, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="8cf1b-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
