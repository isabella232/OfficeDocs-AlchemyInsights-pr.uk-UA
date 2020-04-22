---
title: 2681 напад симулятор в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713487"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="1c8e3-102">Напад симулятор в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1c8e3-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="1c8e3-103">Ви відсутня симулятор нападу?</span><span class="sxs-lookup"><span data-stu-id="1c8e3-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="1c8e3-104">Напад симулятор вимагає **Office 365 розширений загрози захист план 2 (АТФ план 2)** або **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="1c8e3-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="1c8e3-105">Напад симулятор **не** входить до складу Office 365 розширений загрози захист план 1 (АТФ план 1), Office 365 Enterprise E3 або будь-які Microsoft 365 програми для бізнесу підписки.</span><span class="sxs-lookup"><span data-stu-id="1c8e3-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="1c8e3-106">Обліковий запис, який використовується для запуску імітаційні атаки, потребує глобального адміністратора або дозволів адміністратора безпеки та багатофакторної автентифікації (МЗС).</span><span class="sxs-lookup"><span data-stu-id="1c8e3-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="1c8e3-107">Щоб отримати додаткові відомості про вимоги до симулятора атак, перегляньте [цю тему](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="1c8e3-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="1c8e3-108">Важливі речі, щоб знати про **грубої сили** атаки на пароль симуляції:</span><span class="sxs-lookup"><span data-stu-id="1c8e3-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="1c8e3-109">Якщо цільовий обліковий запис, має МЗС, і пароль було здогадалися належним чином, обліковий запис не відображатиметься як скомпрометований (другий фактор автентифікації буде неповним).</span><span class="sxs-lookup"><span data-stu-id="1c8e3-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="1c8e3-110">Розмір файлу пароля не може перевищувати 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="1c8e3-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="1c8e3-111">Використовуйте один пароль на рядок і включіть порожній рядок (повернення каретки) після останнього пароля у списку.</span><span class="sxs-lookup"><span data-stu-id="1c8e3-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="1c8e3-112">Важливі речі, які потрібно знати про **спис фішинг-атак** :</span><span class="sxs-lookup"><span data-stu-id="1c8e3-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="1c8e3-113">За дизайном не можна вказати настроюване значення для **URL-адреси сервера входу фішингового**.</span><span class="sxs-lookup"><span data-stu-id="1c8e3-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="1c8e3-114">Якщо одержувач використовує надбудову для [повідомлення звіту](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , щоб повідомити про фішинг, повідомлення може не з'являтися (оскільки це імітація атаки).</span><span class="sxs-lookup"><span data-stu-id="1c8e3-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="1c8e3-115">Звіти: після того, як моделюється атака завершена, ви можете натиснути **атакувати деталі** , щоб побачити звіт.</span><span class="sxs-lookup"><span data-stu-id="1c8e3-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="1c8e3-116">Докладні інструкції та нові функції в симуляторі атак див. [у Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1c8e3-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
