---
title: Додавання зовнішніх користувачів до групи розсилки
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910953"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="c9cb9-102">Додавання зовнішніх користувачів до групи розсилки</span><span class="sxs-lookup"><span data-stu-id="c9cb9-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="c9cb9-103">Додавання зовнішнього контакту до групи розсилки (DG) – це двоступінний процес:</span><span class="sxs-lookup"><span data-stu-id="c9cb9-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="c9cb9-104">Створити Поштовий контакт для зовнішнього користувача:</span><span class="sxs-lookup"><span data-stu-id="c9cb9-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="c9cb9-105">У центрі адміністрування перейдіть на сторінку[Контакти](https://admin.microsoft.com/adminportal/home#/Contact) **користувачів** > .</span><span class="sxs-lookup"><span data-stu-id="c9cb9-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="c9cb9-106">Виберіть **додати контакт**.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="c9cb9-107">Введіть інформацію про контакт і натисніть **Додати**.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="c9cb9-108">Додати Поштовий контакт до DG:</span><span class="sxs-lookup"><span data-stu-id="c9cb9-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="c9cb9-109">У центрі адміністрування перейдіть > [на сторінку](https://admin.microsoft.com/adminportal/home#/groups) **групи груп.**</span><span class="sxs-lookup"><span data-stu-id="c9cb9-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="c9cb9-110">Знайдіть DG, до якого потрібно додати зовнішнього користувача, і виберіть його, щоб відкрити діалогове вікно редагування.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="c9cb9-111">На вкладці **учасники** виберіть **Переглянути всі та керувати учасниками**.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="c9cb9-112">Виберіть **Додати учасників**.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="c9cb9-113">Виберіть Поштовий контакт, створений на попередньому кроці, і натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="c9cb9-114">Якщо після виконання цих дій зовнішні користувачі не можуть надсилати повідомлення електронної пошти до DG або не отримувати електронні листи від нього, це може бути те, що DG позначено лише дозволити електронні листи від внутрішніх користувачів.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="c9cb9-115">Ви можете перевірити цю конфігурацію і виправити це, дотримуючись вказівок [тут](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="c9cb9-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="c9cb9-116">**Примітка:** Ці інструкції не застосовуються, якщо тип групи "Microsoft 365 групи" замість "групи розсилки".</span><span class="sxs-lookup"><span data-stu-id="c9cb9-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="c9cb9-117">Якщо це так, ви можете додати зовнішній користувач безпосередньо до групи з Outlook.</span><span class="sxs-lookup"><span data-stu-id="c9cb9-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="c9cb9-118">Детальну інформацію про групи Microsoft 365 Гості, а також інструкції щодо додавання зовнішніх гостей можна знайти в [цій статті](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="c9cb9-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  