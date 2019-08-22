---
title: Додавання зовнішніх користувачів до групи розсилки
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494548"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="40ed7-102">Додати зовнішніх користувачів до групи розсилки?</span><span class="sxs-lookup"><span data-stu-id="40ed7-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="40ed7-103">Додавання зовнішній контакт до на розподіл Група (НГ) ІМФ є 2 етапи:</span><span class="sxs-lookup"><span data-stu-id="40ed7-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="40ed7-104">Створення контакту пошти для зовнішніх користувачів:</span><span class="sxs-lookup"><span data-stu-id="40ed7-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="40ed7-105">У центр адміністрування, перейдіть на **користувачів** > сторінці[Контакти](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="40ed7-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="40ed7-106">Виберіть команду **додати контакт**.</span><span class="sxs-lookup"><span data-stu-id="40ed7-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="40ed7-107">Введіть інформацію для вашого контакту та виберіть **Додати**.</span><span class="sxs-lookup"><span data-stu-id="40ed7-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="40ed7-108">Додати Поштовий контакт до вашої DG:</span><span class="sxs-lookup"><span data-stu-id="40ed7-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="40ed7-109">У центр адміністрування, перейдіть до **групи** > сторінці[служби групи](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="40ed7-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="40ed7-110">Знайти DG, щоб додати зовнішній користувачеві і виберіть його, щоб відкрити діалогове вікно редагування.</span><span class="sxs-lookup"><span data-stu-id="40ed7-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="40ed7-111">На вкладці **члени** виберіть **Переглянути всі і керувати членів**.</span><span class="sxs-lookup"><span data-stu-id="40ed7-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="40ed7-112">Виберіть **додати елементи**.</span><span class="sxs-lookup"><span data-stu-id="40ed7-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="40ed7-113">Виберіть Поштовий контакт, який ви створили на попередньому кроці і потім виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="40ed7-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="40ed7-114">Якщо після таких дій зовнішнім користувачам не вдається надіслати електронну пошту до ГД або не отримувати електронні листи від нього, може бути, що ГД позначено лише дозволити електронні листи від внутрішніх користувачів.</span><span class="sxs-lookup"><span data-stu-id="40ed7-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="40ed7-115">Ви можете перевірити цю конфігурацію і виправити її слідом за напрямами [тут](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="40ed7-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="40ed7-116">**Примітка:** Ці інструкції не застосовуються, якщо вашій групі Тип "Office 365 груп» замість «Групи розсилки».</span><span class="sxs-lookup"><span data-stu-id="40ed7-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="40ed7-117">Якщо це так, можна додати зовнішнім користувачем безпосередньо до групи з Outlook.</span><span class="sxs-lookup"><span data-stu-id="40ed7-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="40ed7-118">Детальна інформація про Office 365 груп гостей, а також інструкції з додавання зовнішнього гостей ви знайдете в [цій статті](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="40ed7-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  