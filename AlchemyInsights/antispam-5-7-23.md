---
title: Антиспам-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682346"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="e507d-102">Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="e507d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="e507d-103">Перевірте SPF запис DNS для домену на загальнодоступних SPF або DNS-запис перевірки в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="e507d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="e507d-104">Переконайтеся, що вихідне повідомлення не було визначено як спам, Office 365 і спрямовується через [високий ризик доставки пула](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="e507d-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="e507d-105">Повідомлення в пул з високим ризиком не пройде SPF перевірки, і тому не буде прийнята організація електронної пошти призначення.</span><span class="sxs-lookup"><span data-stu-id="e507d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="e507d-106">Якщо проблема повторюється, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист.</span><span class="sxs-lookup"><span data-stu-id="e507d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="e507d-107">Запишіть докладну зовнішню помилку, доступну в повідомленні відмов.</span><span class="sxs-lookup"><span data-stu-id="e507d-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="e507d-108">Підтримка Office 365 може не бути в змозі допомогти далі.</span><span class="sxs-lookup"><span data-stu-id="e507d-108">Office 365 support may not be able to assist further.</span></span>