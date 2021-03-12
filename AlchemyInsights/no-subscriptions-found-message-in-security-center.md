---
title: У центрі безпеки не знайдено передплату "повідомлення"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "50714392"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="9048b-102">У центрі безпеки не знайдено передплату "повідомлення"</span><span class="sxs-lookup"><span data-stu-id="9048b-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="9048b-103">Якщо під час доступу до центру безпеки захисника Microsoft ви отримуєте повідомлення "не знайдено передплати", це означає, що для входу в портал користувач не має ліцензії на сайт Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="9048b-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="9048b-104">Ліцензії на службу Windows E5 і Office E5 – це окремі ліцензії.</span><span class="sxs-lookup"><span data-stu-id="9048b-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="9048b-105">Відкрийте інцидент підтримки, якщо ліцензію придбано, але не підготовлено до цього екземпляра AAD.</span><span class="sxs-lookup"><span data-stu-id="9048b-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="9048b-106">У вас є:</span><span class="sxs-lookup"><span data-stu-id="9048b-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="9048b-107">Можлива проблема підготовки ліцензії.</span><span class="sxs-lookup"><span data-stu-id="9048b-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="9048b-108">Ви ненавмисно підготування ліцензії до іншої Microsoft AAD, ніж той, який використовується для автентифікації в службі.</span><span class="sxs-lookup"><span data-stu-id="9048b-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>