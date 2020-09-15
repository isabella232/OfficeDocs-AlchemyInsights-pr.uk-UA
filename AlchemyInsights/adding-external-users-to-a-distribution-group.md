---
title: Додавання зовнішніх користувачів до групи розсилки
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663534"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="ad652-102">Додавання зовнішніх користувачів до групи розсилки</span><span class="sxs-lookup"><span data-stu-id="ad652-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="ad652-103">Додавання зовнішнього контакту до групи розсилки (g) – це двоетапний процес:</span><span class="sxs-lookup"><span data-stu-id="ad652-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="ad652-104">Створення поштового контакту для зовнішнього користувача:</span><span class="sxs-lookup"><span data-stu-id="ad652-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="ad652-105">У центрі адміністрування перейдіть на **Users**  >  сторінку[Контакти](https://admin.microsoft.com/adminportal/home#/Contact) користувачів.</span><span class="sxs-lookup"><span data-stu-id="ad652-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="ad652-106">Виберіть елемент **додати контакт**.</span><span class="sxs-lookup"><span data-stu-id="ad652-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="ad652-107">Введіть відомості для вашого контакту та натисніть кнопку **Add (додати**).</span><span class="sxs-lookup"><span data-stu-id="ad652-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="ad652-108">Додавання поштового контакту до програми DГ:</span><span class="sxs-lookup"><span data-stu-id="ad652-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="ad652-109">У центрі адміністрування перейдіть на сторінку **групи груп**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="ad652-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="ad652-110">У розділі DГ потрібно додати зовнішнього користувача, а потім виберіть його, щоб відкрити діалогове вікно редагування.</span><span class="sxs-lookup"><span data-stu-id="ad652-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="ad652-111">На вкладці **учасники** натисніть кнопку **Переглянути всі та керувати учасниками**.</span><span class="sxs-lookup"><span data-stu-id="ad652-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="ad652-112">Виберіть елемент **Додати учасників**.</span><span class="sxs-lookup"><span data-stu-id="ad652-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="ad652-113">Виберіть Поштовий контакт, створений на попередньому кроці, а потім натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="ad652-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="ad652-114">Якщо після виконання цих дій зовнішні користувачі не можуть передавати повідомлення електронної пошти в службу DG або не отримувати електронні листи від нього, це може бути те, що DG позначено, щоб дозволити повідомлення електронної пошти від внутрішніх користувачів.</span><span class="sxs-lookup"><span data-stu-id="ad652-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="ad652-115">Ви можете перевірити цю конфігурацію та вирішити цю проблему, виконавши наведені [нижче вказівки.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="ad652-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="ad652-116">**Примітка.** Ці інструкції не застосовуватимуться, якщо тип групи – "Група Microsoft 365", а не "Група розсилки".</span><span class="sxs-lookup"><span data-stu-id="ad652-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="ad652-117">Якщо це так, ви можете додати зовнішній користувач безпосередньо до групи з програми Outlook.</span><span class="sxs-lookup"><span data-stu-id="ad652-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="ad652-118">Докладні відомості про групи Microsoft 365 Гості, а також інструкції з додавання зовнішніх гостей можна знайти в [цій статті](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="ad652-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  