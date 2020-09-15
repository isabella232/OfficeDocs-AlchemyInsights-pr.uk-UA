---
title: Вирішення проблем із доставкою електронної пошти до спільних папок із підтримкою пошти
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677949"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="acabc-102">Вирішення проблем із доставкою електронної пошти до спільних папок із підтримкою пошти</span><span class="sxs-lookup"><span data-stu-id="acabc-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="acabc-103">Якщо зовнішні відправники не можуть надсилати повідомлення до спільних папок із підтримкою пошти, а відправники отримують повідомлення про помилку: **не вдалося знайти (550 5.4.1)**, переконайтеся, що домен електронної пошти для спільної папки настроєно як внутрішній домен ретрансляції, а не важливий домен:</span><span class="sxs-lookup"><span data-stu-id="acabc-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="acabc-104">Відкрийте [Центр адміністрування Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="acabc-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="acabc-105">Перейдіть на **Mail flow** сторінку \> **допустимі домени**передавання пошти, виберіть допустимий домен і натисніть кнопку **редагувати**.</span><span class="sxs-lookup"><span data-stu-id="acabc-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="acabc-106">На сторінці властивостей, що Відкриється, якщо тип домену має значення " **авторитетний**", змініть значення на **внутрішній ретранслятор** і натисніть кнопку " **зберегти**".</span><span class="sxs-lookup"><span data-stu-id="acabc-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="acabc-107">Якщо зовнішні відправники отримують повідомлення про помилку, у **якому немає дозволу (550 5.7.13)**, виконайте таку команду в [службі Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , щоб переглянути дозволи для анонімних користувачів у спільній папці.</span><span class="sxs-lookup"><span data-stu-id="acabc-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="acabc-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Наприклад, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="acabc-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="acabc-109">Щоб дозволити зовнішнім користувачам надсилати повідомлення електронної пошти до цієї загальнодоступної папки, додайте до анонімного користувача доступ до списку CreateItems.</span><span class="sxs-lookup"><span data-stu-id="acabc-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="acabc-110">Наприклад, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="acabc-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
