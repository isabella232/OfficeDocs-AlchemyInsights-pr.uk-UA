---
title: Антиспам – 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717346"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="27f12-102">Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="27f12-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="27f12-103">Переконайтеся, що запис DNS SPF для вашого домену перебуває в загальнодоступній версії SPF або записі DNS в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="27f12-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="27f12-104">Переконайтеся, що вихідне повідомлення не було визначено як спам від корпорації Майкрософт і маршрутизується через [високий пул доставки ризиків](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="27f12-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="27f12-105">Повідомлення в пулі з високим ризиком не передаватимуться на перевірку SPF, і тому її не буде прийнято організацією електронної пошти призначення.</span><span class="sxs-lookup"><span data-stu-id="27f12-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="27f12-106">Якщо проблему не вирішено, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати повідомлення електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="27f12-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="27f12-107">Зверніть увагу на додаткову зовнішню помилку, доступну в повідомленні відмов.</span><span class="sxs-lookup"><span data-stu-id="27f12-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="27f12-108">Служба підтримки Microsoft може не допомагати надалі.</span><span class="sxs-lookup"><span data-stu-id="27f12-108">Microsoft support may not be able to assist further.</span></span>
