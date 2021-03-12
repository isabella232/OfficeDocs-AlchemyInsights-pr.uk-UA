---
title: Виправлення неполадок із відхилень у програмі Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704915"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="41859-102">Виправлення неполадок із відхилень у програмі Access</span><span class="sxs-lookup"><span data-stu-id="41859-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="41859-103">Якщо хтось отримав повідомлення "відмовлено в доступі" до спільної папки в SharePoint, можливо, адміністратор колекції сайтів дозволив активувати "обмежений доступ до режиму доступу користувачів".</span><span class="sxs-lookup"><span data-stu-id="41859-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="41859-104">Щоб вимкнути цю функцію, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="41859-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="41859-105">Перейдіть на сайт, клацніть піктограму настройки, а потім виберіть пункт **Параметри сайту**.</span><span class="sxs-lookup"><span data-stu-id="41859-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="41859-106">У розділі **адміністрування колекції сайтів** виберіть пункт **функції колекції сайтів**.</span><span class="sxs-lookup"><span data-stu-id="41859-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="41859-107">Поруч із пунктом **заблоковано режим блокування дозволів користувачів "обмежений доступ**" натисніть кнопку **Вимкнути**.</span><span class="sxs-lookup"><span data-stu-id="41859-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="41859-108">Повідомлення про відмову в доступі також може відбутися для спільних папок, якщо сайт – сайт публікації.</span><span class="sxs-lookup"><span data-stu-id="41859-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="41859-109">Щоб отримати докладні дані, у [програмі Access відмовлено в доступі під час доступу до спільної папки](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="41859-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="41859-110">Якщо користувач отримав повідомлення "відмовлено в доступі" під час спроби переглянути запити на доступ, користувачу потрібно додати як адміністратор колекції сайтів або учасник групи "власники" для сайту.</span><span class="sxs-lookup"><span data-stu-id="41859-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="41859-111">Щоб отримати докладніші відомості, перегляньте статтю [Access відмовлено в списку "запити на доступ](https://go.microsoft.com/fwlink/?linkid=2004220)".</span><span class="sxs-lookup"><span data-stu-id="41859-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="41859-112">Якщо користувач отримав повідомлення "відмовлено в доступі" після того, як їх видалено з локальної служби Active Directory, а потім знову додано назад, перегляньте статтю [відмовлено в доступі, коли обліковий запис користувача синхронізується з Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="41859-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

