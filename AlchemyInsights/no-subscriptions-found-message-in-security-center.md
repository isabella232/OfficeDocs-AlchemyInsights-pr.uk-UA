---
title: Повідомлення про те, що передплати не знайдено в Центрі безпеки
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544129"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="3c349-102">Повідомлення про те, що передплати не знайдено в Центрі безпеки</span><span class="sxs-lookup"><span data-stu-id="3c349-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="3c349-103">Якщо під час доступу Центр безпеки для Microsoft Defender з'являється повідомлення "Передплати не знайдено", це означає, що Azure Active Directory (AAD) для входу користувача на портал не має ліцензії ВВП для Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="3c349-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="3c349-104">Ліцензії Windows E5 Office E5 – це окремі ліцензії.</span><span class="sxs-lookup"><span data-stu-id="3c349-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="3c349-105">Відкрийте інцидент підтримки, якщо ліцензію придбано, але не підготовлено для цього екземпляра AAD.</span><span class="sxs-lookup"><span data-stu-id="3c349-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="3c349-106">У вас є:</span><span class="sxs-lookup"><span data-stu-id="3c349-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="3c349-107">Можлива проблема з підготовкою ліцензій.</span><span class="sxs-lookup"><span data-stu-id="3c349-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="3c349-108">Ви ненавмисно підготували ліцензію на іншу службу Microsoft AAD, ніж та, що використовується для автентифікації в службі.</span><span class="sxs-lookup"><span data-stu-id="3c349-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>