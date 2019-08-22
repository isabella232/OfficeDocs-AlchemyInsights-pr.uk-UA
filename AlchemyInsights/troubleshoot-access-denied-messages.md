---
title: 'Усунення проблем: відмовлено у доступі до повідомлення'
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500446"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="8d559-102">Усунення проблем: відмовлено у доступі до повідомлення</span><span class="sxs-lookup"><span data-stu-id="8d559-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="8d559-103">Якщо хтось отримав повідомлення "Немає доступу" до спільної папки в SharePoint, адміністратор колекції сайтів, можливо, ввімкнуто "обмеженим доступом користувача дозволу lockdown режим".</span><span class="sxs-lookup"><span data-stu-id="8d559-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="8d559-104">Щоб вимкнути це:</span><span class="sxs-lookup"><span data-stu-id="8d559-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="8d559-105">Перейдіть до веб-сайту, клацніть піктограму настройки та виберіть пункт **Параметри сайту**.</span><span class="sxs-lookup"><span data-stu-id="8d559-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="8d559-106">Групі **Адміністрування колекції сайтів**виберіть пункт **функцій колекції сайтів**.</span><span class="sxs-lookup"><span data-stu-id="8d559-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="8d559-107">Поруч з **обмеженим доступом користувача дозволу lockdown режимі**натисніть кнопку **Вимкнути**.</span><span class="sxs-lookup"><span data-stu-id="8d559-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="8d559-108">Це повідомлення доступу також може статися для спільних папок, якщо до сайту є сайтом публікації.</span><span class="sxs-lookup"><span data-stu-id="8d559-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="8d559-109">Інформація у розділі [Доступ заборонений, коли доступ до спільної папки](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="8d559-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="8d559-110">Якщо це кому-то повідомлення "Немає доступу" під час спроби переглянути доступ запити, що користувачеві необхідно бути додані як адміністратор колекції сайтів або як член групи власників сайту.</span><span class="sxs-lookup"><span data-stu-id="8d559-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="8d559-111">Для отримання додаткових відомостей див. [Відмовлено в доступі до списку доступу запити](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="8d559-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="8d559-112">Якщо користувач отримав повідомлення "Немає доступу" після того, як вони були видалені з локальної служби Active Directory а потім додати назад, подивитися [Відмовлено в доступі коли облікового запису синхронізовано з Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="8d559-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

