---
title: Заблокуйте підписи електронної пошти, внесені користувачами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243761"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="5660b-102">Заблокуйте підписи електронної пошти, внесені користувачами</span><span class="sxs-lookup"><span data-stu-id="5660b-102">Block user-made email signatures</span></span>

<span data-ttu-id="5660b-103">Таке рішення застосовується лише до підписів електронної пошти, створених в Інтернет-версії Outlook.</span><span class="sxs-lookup"><span data-stu-id="5660b-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="5660b-104">Якщо у вас локальний сервер Exchange, можна заблокувати підписи лише в програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="5660b-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="5660b-105">У центрі адміністрування виберіть пункт Exchange **центри адміністрування**  >  .</span><span class="sxs-lookup"><span data-stu-id="5660b-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="5660b-106">Клацніть **елементи**  >  **політики Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="5660b-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="5660b-107">Виберіть політику, а потім клацніть піктограму олівця, щоб відредагувати її.</span><span class="sxs-lookup"><span data-stu-id="5660b-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="5660b-108">Клацніть **елементи**  >  **Додаткові параметри**.</span><span class="sxs-lookup"><span data-stu-id="5660b-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="5660b-109">У розділі **досвід роботи користувача** зніміть прапорець **підпис електронної пошти** , а потім натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="5660b-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="5660b-110">**Важливо:** Якщо підпис додано, перш ніж зняти цей прапорець, користувач все одно зможе її використовувати.</span><span class="sxs-lookup"><span data-stu-id="5660b-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="5660b-111">Попросіть їх видалити.</span><span class="sxs-lookup"><span data-stu-id="5660b-111">Ask them to remove it.</span></span>
