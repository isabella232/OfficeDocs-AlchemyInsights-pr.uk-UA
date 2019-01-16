---
title: Пересунути повідомлення електронної пошти до поштової скриньки архіву
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319848"
---
<span data-ttu-id="6b85c-p101">Проблеми архівування елементів поштової скриньки архіву. Переконайтеся, що ви виконали наведені нижче кроки:</span><span class="sxs-lookup"><span data-stu-id="6b85c-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="6b85c-p102">Переконайтеся, що **архівувати поштової скриньки** ввімкнено. Якщо ні, то виконайте дії в [цій статті](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) , щоб увімкнути архівну поштову скриньку.</span><span class="sxs-lookup"><span data-stu-id="6b85c-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="6b85c-106">Обмін центру адміністрування виберіть **Теги збереження** під **Управлінням дотримання**, створити **тег збереження** з дією **переміщення до архіву** до потрібного **Терміну збереження**.</span><span class="sxs-lookup"><span data-stu-id="6b85c-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="6b85c-107">Обмін центру адміністрування виберіть **Політики збереження**, створювати **Політику збереження** та додати ваш тег збереження **переміщення до архіву** до цієї політики.</span><span class="sxs-lookup"><span data-stu-id="6b85c-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="6b85c-p103">[Призначити політику збереження](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) до конкретного користувача поштової скриньки. Ту ж політику буде застосовано до **первинної** і поштової скриньки **архіву** .</span><span class="sxs-lookup"><span data-stu-id="6b85c-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="6b85c-p104">Поштову скриньку користувача тепер повинні мати політику архівування для переміщення елементів до поштової скриньки архіву. Можливо, буде необхідно для примусового Керовані папки помічник (МЗС) для запуску і застосувати нові параметри для поштової скриньки користувача. Запустіть таку команду під час [підключення до EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , щоб запустити помічник із керованих папок для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="6b85c-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="6b85c-113">Додаткові відомості про створення політику архівування, див. [Настроювання архіву і видалення політики поштових скриньок](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="6b85c-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

