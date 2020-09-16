---
title: Виправлення неполадок із захистом від підвищення загрози в Office 365 (АТФ)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758086"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="0bf34-102">Виправлення неполадок із АТФ Office 365</span><span class="sxs-lookup"><span data-stu-id="0bf34-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="0bf34-103">**Зверніть увагу на затримку з доставкою повідомлення електронної пошти**?</span><span class="sxs-lookup"><span data-stu-id="0bf34-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="0bf34-104">Скористайтеся параметром динамічної доставки для політик вкладень у службі АТФ.</span><span class="sxs-lookup"><span data-stu-id="0bf34-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="0bf34-105">Після цього ви уникнете затримки доставки повідомлень електронної пошти під час захисту одержувачів від зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="0bf34-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="0bf34-106">**Ви хочете повідомити про помилкові спрацьовувань або помилкових негативів**?</span><span class="sxs-lookup"><span data-stu-id="0bf34-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="0bf34-107">Скористайтеся цим посиланням, щоб надіслати файл для аналізу. [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="0bf34-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="0bf34-108">**Чи знаєте ви, що ви можете ввімкнути захист зв'язків із безпечними посиланнями для електронної пошти, надісланих між користувачами в організації**?</span><span class="sxs-lookup"><span data-stu-id="0bf34-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="0bf34-109">Виконайте наведені нижче кроки.</span><span class="sxs-lookup"><span data-stu-id="0bf34-109">Follow these steps:</span></span>
    1. <span data-ttu-id="0bf34-110">Перейдіть на сторінку https://protection.office.com та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="0bf34-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="0bf34-111">Перехід до **політики керування загрозою**"  >  **Policy**  >  **безпечні посилання**".</span><span class="sxs-lookup"><span data-stu-id="0bf34-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="0bf34-112">У розділі **політики, які стосуються певних одержувачів**, редагування (або додавання) політики.</span><span class="sxs-lookup"><span data-stu-id="0bf34-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="0bf34-113">Виберіть пункт **використовувати безпечні посилання на повідомлення, надіслані в організації**.</span><span class="sxs-lookup"><span data-stu-id="0bf34-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="0bf34-114">Збережіть свою політику та дозвольте приблизно 30 хвилин для змін, які потрібно працювати в центрі обробки даних.</span><span class="sxs-lookup"><span data-stu-id="0bf34-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="0bf34-115">Щоб отримати додаткову довідку з АТФ, перегляньте статтю [захист від розширеної загрози в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="0bf34-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>