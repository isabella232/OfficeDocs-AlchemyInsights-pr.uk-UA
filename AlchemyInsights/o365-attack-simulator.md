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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759240"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="007dd-102">Симулятор атак в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="007dd-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="007dd-103">Не вистачає симулятора атак?</span><span class="sxs-lookup"><span data-stu-id="007dd-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="007dd-104">Для імітатора атак потрібен **пакет захисту від office 365, який має план 2 (АТФ-план 2)** або **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="007dd-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="007dd-105">Тренажер атак **не** входить до складу плану "Office 365 для розширеного захисту від загроз" 1 (план АТФ 1), Office 365 Enterprise E3 або будь-які програми Microsoft 365 для бізнесу.</span><span class="sxs-lookup"><span data-stu-id="007dd-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="007dd-106">Обліковий запис, який використовується для запуску імітованого атак, вимагає використання глобальних дозволів адміністратора або адміністратора системи безпеки та багатофакторної автентифікації (МЗС).</span><span class="sxs-lookup"><span data-stu-id="007dd-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="007dd-107">Докладні відомості про вимоги до симулятора атак наведено в [цій статті](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="007dd-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="007dd-108">Важливі моменти, які потрібно знати про те, як симуляторів атак **грубої сили** .</span><span class="sxs-lookup"><span data-stu-id="007dd-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="007dd-109">Якщо цільовий обліковий запис увімкнуто в МЗС, і пароль було введено неправильно, обліковий запис не відображатиметься як скомпрометований (другий чинник автентифікації буде неповним).</span><span class="sxs-lookup"><span data-stu-id="007dd-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="007dd-110">Розмір файлу пароля не може перевищувати 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="007dd-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="007dd-111">Використовуйте один пароль на одну лінію та включайте пустий рядок (повернення каретки) після останнього пароля у списку.</span><span class="sxs-lookup"><span data-stu-id="007dd-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="007dd-112">Важливі моменти, які потрібно знати про **шахрайство з фішинговим** приєднанним модесом:</span><span class="sxs-lookup"><span data-stu-id="007dd-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="007dd-113">За допомогою макета не можна надавати настроюване значення **URL-адреси сервера входу**.</span><span class="sxs-lookup"><span data-stu-id="007dd-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="007dd-114">Якщо одержувач використовує надбудову " [Увімкнення повідомлення](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) ", щоб повідомити про це повідомлення як фішингове, ви можете не отримувати оповіщення про повідомлення (тому що це імітація атаки).</span><span class="sxs-lookup"><span data-stu-id="007dd-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="007dd-115">Звіти: після завершення імітації атаки можна клацнути елемент **атаки докладно** , щоб переглянути звіт.</span><span class="sxs-lookup"><span data-stu-id="007dd-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="007dd-116">Докладні вказівки та нові функції в імітатор атак наведено [в статті симулятор атак в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="007dd-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
