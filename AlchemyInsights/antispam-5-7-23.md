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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506464"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="39d05-102">Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="39d05-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="39d05-103">Перевірте SPF запис DNS для домену на загальнодоступних SPF або DNS-запис перевірки в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="39d05-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="39d05-104">Переконайтеся, що вихідне повідомлення не було ідентифіковано як спам від корпорації Майкрософт і спрямовується через [пул доставки з високим ризиком](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="39d05-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="39d05-105">Повідомлення в пул з високим ризиком не пройде SPF перевірки, і тому не буде прийнята організація електронної пошти призначення.</span><span class="sxs-lookup"><span data-stu-id="39d05-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="39d05-106">Якщо проблема повторюється, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист.</span><span class="sxs-lookup"><span data-stu-id="39d05-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="39d05-107">Запишіть докладну зовнішню помилку, доступну в повідомленні відмов.</span><span class="sxs-lookup"><span data-stu-id="39d05-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="39d05-108">Служба підтримки Microsoft може не бути в змозі допомогти далі.</span><span class="sxs-lookup"><span data-stu-id="39d05-108">Microsoft support may not be able to assist further.</span></span>
