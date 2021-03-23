---
title: Захист від атаки Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037183"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="59d0a-102">Захист від атаки Backscatter</span><span class="sxs-lookup"><span data-stu-id="59d0a-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="59d0a-103">Backscatter – це звіти про недоставку (також відомі як NDRs або Bounce повідомлення), які ви отримали для повідомлень, які не надсилали.</span><span class="sxs-lookup"><span data-stu-id="59d0a-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="59d0a-104">Спамери Forge (пародія) **від:** адреса своїх повідомлень, і вони часто використовують реальні адреси електронної пошти, щоб надати довіру до своїх повідомлень.</span><span class="sxs-lookup"><span data-stu-id="59d0a-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="59d0a-105">Таким чином, коли спамери неминуче надсилають повідомлення неіснуючим одержувачам, поштовий сервер призначення суттєво обманом повертає повідомлення, що не вдалося знайти в повідомленні про НЕДОСТАВКУ, до кованого відправника в адресі **From:** Address (адреса).</span><span class="sxs-lookup"><span data-stu-id="59d0a-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="59d0a-106">Додаткові відомості можна знайти в [Backscatter в EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="59d0a-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="59d0a-107">**Увімкнення захисту від Backscatter**</span><span class="sxs-lookup"><span data-stu-id="59d0a-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="59d0a-108">Щоб увімкнути захист Backscatter, виконайте наведені нижче вказівки.</span><span class="sxs-lookup"><span data-stu-id="59d0a-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="59d0a-109">**protection.office.com > керування загрозою > політики > антиспам > виберіть політику фільтра спаму та редагувати політику > спам-властивості > позначки як спам > НЕДОСТАВКУ Backscatter > установіть його на "увімкнуто"**</span><span class="sxs-lookup"><span data-stu-id="59d0a-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="59d0a-110">Якщо ви вважаєте, що обліковий запис було скомпрометовано, ознайомтеся з такими:</span><span class="sxs-lookup"><span data-stu-id="59d0a-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="59d0a-111">Відповідь на несанкціонований обліковий запис електронної пошти</span><span class="sxs-lookup"><span data-stu-id="59d0a-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="59d0a-112">Видалення заблокованих користувачів із порталу обмеженого користувача в Office 365</span><span class="sxs-lookup"><span data-stu-id="59d0a-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



