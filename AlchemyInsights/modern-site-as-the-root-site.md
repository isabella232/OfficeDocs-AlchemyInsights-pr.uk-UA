---
title: Сучасний сайт як корінь сайту
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057795"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="58586-102">Сучасний сайт як корінь сайту</span><span class="sxs-lookup"><span data-stu-id="58586-102">Modern site as root site</span></span>

<span data-ttu-id="58586-103">[Випуск цільових](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) клієнтів тепер можна ввімкнути досвід новітні комунікаційно сайту на сайт класичні корінь їх компонентів SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58586-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="58586-104">Ця функція може бути активований, запустивши на командлета простий PowerShell.</span><span class="sxs-lookup"><span data-stu-id="58586-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="58586-105">Успішне виконання PowerShell command(s) корінь сайту буде мати нову домашню сторінку сайту спілкування.</span><span class="sxs-lookup"><span data-stu-id="58586-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="58586-106">Подробиці про PowerShell командлета вимоги до та функції доступні у статті [Увімкнення SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="58586-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="58586-107">Ми будемо поступово прокату це, вимкнено за промовчанням клієнтам цільової звільнення на початку травня 2019, і рулон на будуть доступні по всьому світу до кінця червня 2019.</span><span class="sxs-lookup"><span data-stu-id="58586-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="58586-108">Як і раніше, зверніться до [Центру повідомлення](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) для інших нових функцій із сучасним.</span><span class="sxs-lookup"><span data-stu-id="58586-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="58586-109">**Важливо**: не видалити ваш класичний кореневий сайт для створення сучасного повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="58586-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="58586-110">Це не підтримується корпорацією Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="58586-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="58586-111">Видалення кореневий сайт буде зробити всі сайти SharePoint у вашій організації недоступними для всіх користувачів, доки ви не відновити сайту або створіть новий сайт в той же URL.</span><span class="sxs-lookup"><span data-stu-id="58586-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 