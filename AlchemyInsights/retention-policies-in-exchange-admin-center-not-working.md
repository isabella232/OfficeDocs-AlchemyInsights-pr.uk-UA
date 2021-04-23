---
title: Політики збереження в Центрі адміністрування Exchange не працюють
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952249"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="33bb6-102">Політики збереження в Центрі адміністрування Exchange</span><span class="sxs-lookup"><span data-stu-id="33bb6-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="33bb6-103">Якщо ви хочете, щоб ми виконували автоматичні перевірки наведених нижче параметрів, натисніть кнопку "Назад" < – у верхній частині цієї сторінки, а потім введіть адресу електронної пошти користувача, який має проблеми з політиками збереження.</span><span class="sxs-lookup"><span data-stu-id="33bb6-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="33bb6-104">Якщо виникають проблеми з політиками збереження в Центрі адміністрування Exchange, які не застосовуються до поштових скриньок або елементів, які не переміщуються до архівної поштової скриньки, перевірте таке:</span><span class="sxs-lookup"><span data-stu-id="33bb6-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="33bb6-105">**Причини:**</span><span class="sxs-lookup"><span data-stu-id="33bb6-105">**Root Causes:**</span></span>

- <span data-ttu-id="33bb6-106">**Помічник із керованих** папок не обробив поштову скриньку користувача.</span><span class="sxs-lookup"><span data-stu-id="33bb6-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="33bb6-107">Помічник із керованих папок намагається обробляти кожну поштову скриньку в хмарній організації один раз на сім днів.</span><span class="sxs-lookup"><span data-stu-id="33bb6-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="33bb6-108">**Вирішення.** Запустіть помічник із керованих папок.</span><span class="sxs-lookup"><span data-stu-id="33bb6-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="33bb6-109">**RetentionHold** **увімкнуто** в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="33bb6-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="33bb6-110">Якщо поштову скриньку розміщено в Політиці збереження, політика збереження для поштової скриньки не оброблятимуться в цей час.</span><span class="sxs-lookup"><span data-stu-id="33bb6-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="33bb6-111">**Вирішення.** Перевірте стан параметра утримання та оновіть його за потреби.</span><span class="sxs-lookup"><span data-stu-id="33bb6-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="33bb6-112">Докладні відомості див. у [утримання поштової скриньки.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="33bb6-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="33bb6-113">**Примітка.** Якщо розмір поштової скриньки менше 10 МБ, помічник із керованих папок не обробить поштову скриньку автоматично.</span><span class="sxs-lookup"><span data-stu-id="33bb6-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="33bb6-114">Докладні відомості про політики збереження в Центрі адміністрування Exchange див. у розділах:</span><span class="sxs-lookup"><span data-stu-id="33bb6-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="33bb6-115">Позначки та політики збереження</span><span class="sxs-lookup"><span data-stu-id="33bb6-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="33bb6-116">[Застосування політики збереження до поштових скриньок](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) або [додавання або видалення позначок збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="33bb6-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="33bb6-117">Визначення типу утримання, розміщеного в поштовій скриньці</span><span class="sxs-lookup"><span data-stu-id="33bb6-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
