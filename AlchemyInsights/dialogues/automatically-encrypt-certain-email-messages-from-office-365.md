---
title: Автоматичне шифрування певних повідомлень електронної пошти з Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527623"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="45105-102">Автоматичне шифрування певних повідомлень електронної пошти з Office 365</span><span class="sxs-lookup"><span data-stu-id="45105-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="45105-103">У [центрі адміністрування Exchange](https://outlook.office365.com/ecp/)виберіть пункт **правила передавання пошти >**.</span><span class="sxs-lookup"><span data-stu-id="45105-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="45105-104">Клацніть піктограму **Створити (+)** , а потім виберіть команду "**Додати шифрування повідомлень Office 365" і "захист прав" до повідомлень**.</span><span class="sxs-lookup"><span data-stu-id="45105-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="45105-105">У полі **ім'я** введіть ім'я для правила, наприклад *шифрувати всі повідомлення*.</span><span class="sxs-lookup"><span data-stu-id="45105-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="45105-106">У **разі використання цього правила** натисніть кнопку **[застосувати до всіх повідомлень]**.</span><span class="sxs-lookup"><span data-stu-id="45105-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="45105-107">Поруч із полем **виконати наведені нижче дії** натисніть кнопку **вибрати один**.</span><span class="sxs-lookup"><span data-stu-id="45105-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="45105-108">У розкривному меню **шаблон RMS** виберіть пункт **Зашифрувати**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="45105-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="45105-109">(Якщо цей параметр не відображається, це означає, що план не містить автоматичного шифрування.</span><span class="sxs-lookup"><span data-stu-id="45105-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="45105-110">Але його можна додати!)</span><span class="sxs-lookup"><span data-stu-id="45105-110">But you can add it!)</span></span>
7. <span data-ttu-id="45105-111">Установіть прапорець **відстеження цього правила з рівнем важливості** , а потім виберіть потрібний рівень.</span><span class="sxs-lookup"><span data-stu-id="45105-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="45105-112">Якщо ваша компанія має договірні зобов'язання надіслати всі зашифровані повідомлення електронної пошти, радимо встановити **високий** рівень.</span><span class="sxs-lookup"><span data-stu-id="45105-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="45105-113">У розділі **вибір моделі для цього правила** натисніть кнопку **Застосувати**.</span><span class="sxs-lookup"><span data-stu-id="45105-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="45105-114">Виберіть будь-яке необов'язкове виділення (зі списку необов'язкових варіантів, які можна зробити в цій точці, багато з яких можна використовувати за замовчуванням для простоти).</span><span class="sxs-lookup"><span data-stu-id="45105-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="45105-115">Натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="45105-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="45105-116">Ви завжди можете повернутися та відредагувати це правило згодом.</span><span class="sxs-lookup"><span data-stu-id="45105-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="45105-117">Докладні відомості про створення правил для шифрування наведено в статті [визначення правил передавання пошти для шифрування повідомлень електронної пошти в Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="45105-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

