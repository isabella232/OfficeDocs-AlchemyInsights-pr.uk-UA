---
title: Виправлення неполадок із захистом Office 365 для підвищення загрози
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658935"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="d25fc-102">Виправлення неполадок із захистом Office 365 для підвищення загрози</span><span class="sxs-lookup"><span data-stu-id="d25fc-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="d25fc-103">Чи помітили ви затримки в доставці повідомлень?</span><span class="sxs-lookup"><span data-stu-id="d25fc-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="d25fc-104">Використовуйте параметр [динамічної доставки](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) в політиці вкладень у сейфі АТФ.</span><span class="sxs-lookup"><span data-stu-id="d25fc-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="d25fc-105">Це дасть змогу уникнути затримок повідомлень під час захисту одержувачів від зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="d25fc-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="d25fc-106">Ви хочете повідомити про помилкові спрацьовування або помилкові негативи в корпорацію Майкрософт?</span><span class="sxs-lookup"><span data-stu-id="d25fc-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="d25fc-107">Використовуйте це [посилання](https://www.microsoft.com/wdsi/filesubmission/) , щоб надсилати файли для аналізу.</span><span class="sxs-lookup"><span data-stu-id="d25fc-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="d25fc-108">Чи знаєте ви, що можна активувати захист для внутрішнього повідомлення електронної пошти, надіслане між одержувачами в організації?</span><span class="sxs-lookup"><span data-stu-id="d25fc-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="d25fc-109">Виконайте наведені нижче кроки.</span><span class="sxs-lookup"><span data-stu-id="d25fc-109">Follow these steps:</span></span>

  1. <span data-ttu-id="d25fc-110">Перейдіть на сторінку [https://protection.office.com](https://protection.office.com) та увійдіть за допомогою облікового запису глобального адміністратора або адміністратора безпеки.</span><span class="sxs-lookup"><span data-stu-id="d25fc-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="d25fc-111">В області переходів ліворуч у розділі **керування загрозою**виберіть посилання **політики** \> **безпеки**.</span><span class="sxs-lookup"><span data-stu-id="d25fc-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="d25fc-112">У розділі політики, **які застосовуватимуться до всієї організації** , виберіть політику та натисніть кнопку **редагувати**.</span><span class="sxs-lookup"><span data-stu-id="d25fc-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="d25fc-113">У розділі **Параметри**Увімкніть параметр **використовувати безпечні посилання на повідомлення, надіслані в організації**.</span><span class="sxs-lookup"><span data-stu-id="d25fc-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
