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
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483361"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="2d6c6-102">Заблокуйте підписи електронної пошти, внесені користувачами</span><span class="sxs-lookup"><span data-stu-id="2d6c6-102">Block user-made email signatures</span></span>

<span data-ttu-id="2d6c6-103">Таке рішення застосовується лише до підписів електронної пошти, створених в Інтернет-версії Outlook.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="2d6c6-104">Якщо у вас локальний сервер Exchange, можна заблокувати підписи лише в програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="2d6c6-105">У центрі адміністрування виберіть пункт Exchange **центри адміністрування**  >  .</span><span class="sxs-lookup"><span data-stu-id="2d6c6-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="2d6c6-106">Клацніть **елементи**  >  **політики Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="2d6c6-107">Виберіть політику, а потім клацніть піктограму олівця, щоб відредагувати її.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="2d6c6-108">Клацніть **елементи**  >  **Додаткові параметри**.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="2d6c6-109">У розділі **досвід роботи користувача** зніміть прапорець **підпис електронної пошти** , а потім натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="2d6c6-110">**Важливо:** Якщо підпис додано, перш ніж зняти цей прапорець, користувач все одно зможе її використовувати.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="2d6c6-111">Попросіть їх видалити.</span><span class="sxs-lookup"><span data-stu-id="2d6c6-111">Ask them to remove it.</span></span>
