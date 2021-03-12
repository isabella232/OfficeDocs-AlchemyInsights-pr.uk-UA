---
title: Автоматичне шифрування певних повідомлень електронної пошти Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749449"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="bb6a7-102">Автоматичне шифрування певних повідомлень електронної пошти Office 365</span><span class="sxs-lookup"><span data-stu-id="bb6a7-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="bb6a7-103">Ви можете автоматично шифрувати повідомлення, які користувачі надсилають певним зовнішнім користувачам або організаціям.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="bb6a7-104">Для цього виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="bb6a7-105">У [центрі адміністрування Exchange](https://outlook.office365.com/ecp/)виберіть пункт **правила передавання пошти >**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="bb6a7-106">Клацніть піктограму **Створити (+)** , а потім виберіть команду "**Додати шифрування повідомлень Office 365" і "захист прав" до повідомлень**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="bb6a7-107">У полі **ім'я** введіть ім'я для правила, наприклад *шифрувати повідомлення, надіслані до DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="bb6a7-108">У **разі використання цього правила, якщо** вибрати **одержувача > цей користувач**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="bb6a7-109">У вікні **вибір учасників** виберіть ім'я особи, до якої потрібно застосувати правило шифрування, і натисніть кнопку **Додати**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="bb6a7-110">Завершивши додавання користувачів, натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="bb6a7-111">Поруч із полем **виконати наведені нижче дії** натисніть кнопку **вибрати один**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="bb6a7-112">У розкривному меню **шаблон RMS** виберіть пункт **Зашифрувати**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="bb6a7-113">(Якщо цей параметр не відображається, це означає, що план не містить автоматичного шифрування.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="bb6a7-114">Але його можна додати!)</span><span class="sxs-lookup"><span data-stu-id="bb6a7-114">But you can add it!)</span></span>
9. <span data-ttu-id="bb6a7-115">Виберіть будь-яке необов'язкове виділення (зі списку необов'язкових варіантів, які можна зробити в цій точці, багато з яких можна використовувати за замовчуванням для простоти).</span><span class="sxs-lookup"><span data-stu-id="bb6a7-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="bb6a7-116">Натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bb6a7-117">Ви завжди можете повернутися та відредагувати це правило згодом.</span><span class="sxs-lookup"><span data-stu-id="bb6a7-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="bb6a7-118">Щоб отримати докладні відомості про створення правил для шифрування, Дізнайтеся, як [визначити правила передавання пошти для шифрування повідомлень електронної пошти в Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="bb6a7-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

