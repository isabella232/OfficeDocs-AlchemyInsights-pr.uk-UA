---
title: Автоматичне шифрування повідомлень електронної пошти Office 365, надісланих до певних доменів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749296"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="bb8b1-102">Автоматичне шифрування повідомлень електронної пошти Office 365, надісланих до певних доменів</span><span class="sxs-lookup"><span data-stu-id="bb8b1-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="bb8b1-103">У [центрі адміністрування Exchange](https://outlook.office365.com/ecp/)виберіть пункт **правила передавання пошти >**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="bb8b1-104">Клацніть піктограму **Створити (+)** , а потім виберіть команду "**Додати шифрування повідомлень Office 365" і "захист прав" до повідомлень**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="bb8b1-105">У полі **ім'я** введіть ім'я для правила, наприклад *шифрувати повідомлення, надіслані до contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="bb8b1-106">У **разі використання цього правила** виберіть **домен > одержувача**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="bb8b1-107">Введіть ім'я домену, наприклад **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="bb8b1-108">Клацніть піктограму **Add (+)** , а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="bb8b1-109">Поруч із полем **виконати наведені нижче дії** натисніть кнопку **вибрати один**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="bb8b1-110">У розкривному меню **шаблон RMS** виберіть пункт **Зашифрувати**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="bb8b1-111">(Якщо цей параметр не відображається, це означає, що план не містить автоматичного шифрування.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="bb8b1-112">Але його можна додати!)</span><span class="sxs-lookup"><span data-stu-id="bb8b1-112">But you can add it!)</span></span>
9. <span data-ttu-id="bb8b1-113">Виберіть будь-яке необов'язкове виділення (зі списку необов'язкових варіантів, які можна зробити в цій точці, багато з яких можна використовувати за замовчуванням для простоти).</span><span class="sxs-lookup"><span data-stu-id="bb8b1-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="bb8b1-114">Натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bb8b1-115">Ви завжди можете повернутися та відредагувати це правило згодом.</span><span class="sxs-lookup"><span data-stu-id="bb8b1-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="bb8b1-116">Докладні відомості про створення правил для шифрування наведено в статті [визначення правил передавання пошти для шифрування повідомлень електронної пошти в Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="bb8b1-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>