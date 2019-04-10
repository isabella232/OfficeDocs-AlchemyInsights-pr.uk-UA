---
title: Пересунути повідомлення електронної пошти до поштової скриньки архіву
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747224"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="0dede-102">Переміщення електронної пошти до поштової скриньки архіву</span><span class="sxs-lookup"><span data-stu-id="0dede-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="0dede-103">Переконайтеся, що **архівувати поштової скриньки** ввімкнено.</span><span class="sxs-lookup"><span data-stu-id="0dede-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="0dede-104">Якщо ні, скориставшись вказівками в [цій статті](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) увімкнення поштової скриньки архіву.</span><span class="sxs-lookup"><span data-stu-id="0dede-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="0dede-105">Щоб заархівувати повідомлення автоматично до поштової скриньки архіву, тег збереження з **перемістити до архіву** дії слід установити **застосовуються автоматично до всієї поштової скриньки (за замовчуванням) тег**.</span><span class="sxs-lookup"><span data-stu-id="0dede-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="0dede-106">Виконайте дії тут, щоб створити тег: [Тег архіву за промовчанням](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="0dede-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="0dede-107">Далі, додати **Архів** тегів політики збереження.</span><span class="sxs-lookup"><span data-stu-id="0dede-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="0dede-108">У центру адміністрування Exchange виберіть **Політики збереження** > доповнити **перемістити до архіву тег** політики > **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="0dede-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="0dede-109">Тепер [призначити політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) конкретного користувача поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="0dede-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="0dede-110">Ту ж політику буде застосовано до **первинної** і поштової скриньки **архіву** .</span><span class="sxs-lookup"><span data-stu-id="0dede-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="0dede-111">Можливо, буде необхідно для примусового Керовані папки помічник (МЗС) для запуску і застосувати нові параметри для поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="0dede-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="0dede-112">Запустіть таку команду під час [підключення до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , щоб запустити помічник із керованих папок для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="0dede-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="0dede-113">Щоб отримати додаткові відомості про налаштування політику архівування переглянути [набір до архіву і видалення політики поштових скриньок](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="0dede-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

