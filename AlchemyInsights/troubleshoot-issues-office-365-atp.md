---
title: Усунення проблем, пов'язаних з Office 365 розширений захист від загроз (АТФ)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511133"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="de3dd-102">Виправлення неполадок, пов'язаних із АТФ Office 365</span><span class="sxs-lookup"><span data-stu-id="de3dd-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="de3dd-103">**Зверніть увагу на затримки з доставкою повідомлень електронної пошти**?</span><span class="sxs-lookup"><span data-stu-id="de3dd-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="de3dd-104">Спробуйте скористатися варіантом динамічного доставки для політики безпечних вкладень АТФ.</span><span class="sxs-lookup"><span data-stu-id="de3dd-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="de3dd-105">Це дозволить уникнути затримки доставки повідомлень електронної пошти, захищаючи одержувачів від шкідливих файлів.</span><span class="sxs-lookup"><span data-stu-id="de3dd-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="de3dd-106">**Ви хочете повідомити про помилкове спрацьовування або помилкові негативи**?</span><span class="sxs-lookup"><span data-stu-id="de3dd-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="de3dd-107">Скористайтеся цим посиланням для надсилання файлу для аналізу:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="de3dd-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="de3dd-108">**Чи знаєте ви, що ви можете увімкнути захист безпечних ЗВ'ЯЗКІВ АТФ для електронної пошти, що надсилається між людьми в організації**?</span><span class="sxs-lookup"><span data-stu-id="de3dd-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="de3dd-109">Виконайте наведені нижче кроки.</span><span class="sxs-lookup"><span data-stu-id="de3dd-109">Follow these steps:</span></span>
    1. <span data-ttu-id="de3dd-110">Перейдіть до https://protection.office.com і ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="de3dd-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="de3dd-111">Перейдіть до **політики керування загрозами**  >  **Policy**  >  **безпечні посилання**.</span><span class="sxs-lookup"><span data-stu-id="de3dd-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="de3dd-112">У розділі **політики, які застосовуються до певних одержувачів**, змінити (або додати) політику.</span><span class="sxs-lookup"><span data-stu-id="de3dd-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="de3dd-113">Виберіть " **Застосувати безпечні посилання" до повідомлень, надісланих в межах організації**.</span><span class="sxs-lookup"><span data-stu-id="de3dd-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="de3dd-114">Збережіть свою політику та дозвольте близько 30 хвилин, щоб ваші зміни працювали через ваш центр обробки даних.</span><span class="sxs-lookup"><span data-stu-id="de3dd-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="de3dd-115">Щоб отримати додаткову довідку з АТФ, перегляньте [Office 365 розширений захист від загроз](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="de3dd-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>