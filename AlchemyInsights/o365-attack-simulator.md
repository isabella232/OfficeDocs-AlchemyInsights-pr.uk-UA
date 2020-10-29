---
title: Симулятор атак 2681 у Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801572"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="524d2-102">Симулятор атак в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="524d2-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="524d2-103">Не вистачає симулятора атак?</span><span class="sxs-lookup"><span data-stu-id="524d2-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="524d2-104">Для імітатора атак потрібен **захисник Microsoft для Office 365 (план АТФ 2)** або **Office 365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="524d2-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="524d2-105">Тренажер атак **не** входить до складу Microsoft Defender для Office 365 (план АТФ 1), Office 365 Enterprise E3 або будь-які програми Microsoft 365 для бізнесу.</span><span class="sxs-lookup"><span data-stu-id="524d2-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="524d2-106">Обліковий запис, який використовується для запуску імітованого атак, вимагає використання глобальних дозволів адміністратора або адміністратора системи безпеки та багатофакторної автентифікації (МЗС).</span><span class="sxs-lookup"><span data-stu-id="524d2-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="524d2-107">Докладні відомості про вимоги до симулятора атак наведено в [цій статті](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="524d2-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="524d2-108">Важливі моменти, які потрібно знати про те, як симуляторів атак **грубої сили** .</span><span class="sxs-lookup"><span data-stu-id="524d2-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="524d2-109">Якщо цільовий обліковий запис увімкнуто в МЗС, і пароль було введено неправильно, обліковий запис не відображатиметься як скомпрометований (другий чинник автентифікації буде неповним).</span><span class="sxs-lookup"><span data-stu-id="524d2-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="524d2-110">Розмір файлу пароля не може перевищувати 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="524d2-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="524d2-111">Використовуйте один пароль на одну лінію та включайте пустий рядок (повернення каретки) після останнього пароля у списку.</span><span class="sxs-lookup"><span data-stu-id="524d2-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="524d2-112">Важливі моменти, які потрібно знати про **шахрайство з фішинговим** приєднанним модесом:</span><span class="sxs-lookup"><span data-stu-id="524d2-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="524d2-113">За допомогою макета не можна надавати настроюване значення **URL-адреси сервера входу** .</span><span class="sxs-lookup"><span data-stu-id="524d2-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="524d2-114">Якщо одержувач використовує надбудову " [Увімкнення повідомлення](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) ", щоб повідомити про це повідомлення як фішингове, ви можете не отримувати оповіщення про повідомлення (тому що це імітація атаки).</span><span class="sxs-lookup"><span data-stu-id="524d2-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="524d2-115">Звіти: після завершення імітації атаки можна клацнути елемент **атаки докладно** , щоб переглянути звіт.</span><span class="sxs-lookup"><span data-stu-id="524d2-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="524d2-116">Докладні вказівки та нові функції в імітатор атак наведено [в статті симулятор атак в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="524d2-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
