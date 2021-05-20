---
title: 2681 Симулятор атаки в Microsoft 365
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545747"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="42aa4-102">Моделятор атаки в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="42aa4-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="42aa4-103">Не бракує симулятора атаки?</span><span class="sxs-lookup"><span data-stu-id="42aa4-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="42aa4-104">Для моделювання атаки потрібен **Захисник Microsoft Office 365 (план 2** **або Office 365 для підприємств E5).**</span><span class="sxs-lookup"><span data-stu-id="42aa4-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="42aa4-105">Моделятор  атаки не входить до складу Microsoft Defender Office 365 (план 1), Office 365 для підприємств E3 або будь-Програми Microsoft 365 для бізнесу передплати.</span><span class="sxs-lookup"><span data-stu-id="42aa4-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="42aa4-106">Для запуску зімітованих атак облікового запису потрібні дозволи глобального адміністратора або адміністратора безпеки та багатофакторна автентифікація (MFA).</span><span class="sxs-lookup"><span data-stu-id="42aa4-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="42aa4-107">Докладні відомості про вимоги до моделювання атаки див. [в цій статті.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="42aa4-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="42aa4-108">Важливі відомості про **Brute Force Password attack** simulations:</span><span class="sxs-lookup"><span data-stu-id="42aa4-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="42aa4-109">Якщо для цільового облікового запису активовано багатофакторну автентифікацію, а пароль вдасться вгадати правильно, обліковий запис не відображатимуться як злам (другий фактор автентифікації буде неповний).</span><span class="sxs-lookup"><span data-stu-id="42aa4-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="42aa4-110">Розмір файлу пароля не має бути більше 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="42aa4-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="42aa4-111">У кожного рядка слід використовувати один пароль і включати пустий рядок (повернення карети) після останнього пароля в списку.</span><span class="sxs-lookup"><span data-stu-id="42aa4-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="42aa4-112">Важливі відомості про **моделювання фішингів:**</span><span class="sxs-lookup"><span data-stu-id="42aa4-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="42aa4-113">За задумом не можна вказати настроюване значення для URL-адреси сервера **фішинг для входу.**</span><span class="sxs-lookup"><span data-stu-id="42aa4-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="42aa4-114">Якщо одержувач використовує [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) надбудову "Активувати звіт про повідомлення", щоб повідомити про фішинг, повідомлення може не надійти (оскільки це зімітована атака).</span><span class="sxs-lookup"><span data-stu-id="42aa4-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="42aa4-115">Звіти. Після зімітованої атаки можна натиснути кнопку Відомості про **атаку,** щоб переглянути звіт.</span><span class="sxs-lookup"><span data-stu-id="42aa4-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="42aa4-116">Докладні інструкції та нові функції в симуляторі атаки див. в статті [Моделятор атаки Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="42aa4-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
