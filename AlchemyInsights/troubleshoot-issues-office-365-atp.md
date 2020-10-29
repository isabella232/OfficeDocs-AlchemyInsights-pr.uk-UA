---
title: Усунення несправностей із програмою Microsoft Defender для Office 365 (АТФ)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801428"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="777c6-102">Виправлення неполадок із АТФ Office 365</span><span class="sxs-lookup"><span data-stu-id="777c6-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="777c6-103">**Зверніть увагу на затримку з доставкою повідомлення електронної пошти** ?</span><span class="sxs-lookup"><span data-stu-id="777c6-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="777c6-104">Скористайтеся параметром динамічної доставки для політик вкладень у службі АТФ.</span><span class="sxs-lookup"><span data-stu-id="777c6-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="777c6-105">Після цього ви уникнете затримки доставки повідомлень електронної пошти під час захисту одержувачів від зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="777c6-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="777c6-106">**Ви хочете повідомити про помилкові спрацьовувань або помилкових негативів** ?</span><span class="sxs-lookup"><span data-stu-id="777c6-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="777c6-107">Скористайтеся цим посиланням, щоб надіслати файл для аналізу. [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="777c6-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="777c6-108">**Чи знаєте ви, що ви можете ввімкнути захист зв'язків із безпечними посиланнями для електронної пошти, надісланих між користувачами в організації** ?</span><span class="sxs-lookup"><span data-stu-id="777c6-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="777c6-109">Виконайте наведені нижче кроки.</span><span class="sxs-lookup"><span data-stu-id="777c6-109">Follow these steps:</span></span>
    1. <span data-ttu-id="777c6-110">Перейдіть на сторінку https://protection.office.com та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="777c6-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="777c6-111">Перехід до **політики керування загрозою** "  >  **Policy**  >  **безпечні посилання** ".</span><span class="sxs-lookup"><span data-stu-id="777c6-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="777c6-112">У розділі **політики, які стосуються певних одержувачів** , редагування (або додавання) політики.</span><span class="sxs-lookup"><span data-stu-id="777c6-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="777c6-113">Виберіть пункт **використовувати безпечні посилання на повідомлення, надіслані в організації** .</span><span class="sxs-lookup"><span data-stu-id="777c6-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="777c6-114">Збережіть свою політику та дозвольте приблизно 30 хвилин для змін, які потрібно працювати в центрі обробки даних.</span><span class="sxs-lookup"><span data-stu-id="777c6-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="777c6-115">Щоб отримати додаткову довідку з АТФ, перегляньте статтю [Microsoft Defender для Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="777c6-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>