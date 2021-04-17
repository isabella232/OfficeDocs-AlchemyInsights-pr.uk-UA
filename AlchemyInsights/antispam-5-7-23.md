---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821432"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="5aeb3-102">Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="5aeb3-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="5aeb3-103">Перевірте запис DNS SPF для свого домену в загальнодоступному перевіркі записів SPF або DNS в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="5aeb3-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="5aeb3-104">Переконайтеся, що корпорація Майкрософт не визначила вихідне повідомлення як спам і направила його через пул доставки з високим [ризиком.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="5aeb3-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="5aeb3-105">Повідомлення в пулі доставки з високим ризиком не проходять перевірки SPF, тому не прийматимуться цільовою організацією електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="5aeb3-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="5aeb3-106">Якщо проблема не зникне, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист.</span><span class="sxs-lookup"><span data-stu-id="5aeb3-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="5aeb3-107">Занотувати докладну зовнішню помилку, доступну в звіті про незабаром.</span><span class="sxs-lookup"><span data-stu-id="5aeb3-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="5aeb3-108">Можливо, службі підтримки Microsoft не вдасться допомогти.</span><span class="sxs-lookup"><span data-stu-id="5aeb3-108">Microsoft support may not be able to assist further.</span></span>
