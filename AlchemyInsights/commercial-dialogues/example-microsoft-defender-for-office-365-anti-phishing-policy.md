---
title: Приклад захисту від фішинг-махінацій Microsoft для Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750801"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="14c78-102">Приклад захисту від фішинг-махінацій Microsoft для Office 365</span><span class="sxs-lookup"><span data-stu-id="14c78-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="14c78-103">Ці параметри дають змогу політиці під назвою " *домен і головний виконавчий директор*".</span><span class="sxs-lookup"><span data-stu-id="14c78-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="14c78-104">Ця політика забезпечує захист користувачів і доменів від уособлення, а потім застосовує політику до всіх повідомлень електронної пошти, отриманих користувачами в домені.</span><span class="sxs-lookup"><span data-stu-id="14c78-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="14c78-105">Спочатку додайте наведені нижче відомості, щоб створити політику.</span><span class="sxs-lookup"><span data-stu-id="14c78-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="14c78-106">**Ім'я**: домен і CEO **Опис**: гарантує, що Генеральний директор і ваш домен не уособлюються.</span><span class="sxs-lookup"><span data-stu-id="14c78-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="14c78-107">**Застосувати до**: виберіть **домен одержувача**.</span><span class="sxs-lookup"><span data-stu-id="14c78-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="14c78-108">У розділі **будь-якого з цих** виберіть пункт **вибрати**, а потім виберіть домен.</span><span class="sxs-lookup"><span data-stu-id="14c78-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="14c78-109">Виберіть **+ Add (додати**).</span><span class="sxs-lookup"><span data-stu-id="14c78-109">Select **+ Add**.</span></span> <span data-ttu-id="14c78-110">Установіть прапорець біля імені домену в списку (наприклад, *contoso.com*), а потім натисніть кнопку **Add (додати**).</span><span class="sxs-lookup"><span data-stu-id="14c78-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="14c78-111">Натисніть кнопку " **виконати**".</span><span class="sxs-lookup"><span data-stu-id="14c78-111">Select **Done**.</span></span>
- <span data-ttu-id="14c78-112">Після створення політики можна точно настроїти політику за допомогою наведених нижче параметрів.</span><span class="sxs-lookup"><span data-stu-id="14c78-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="14c78-113">**Додавання користувачів до захисту:** У цьому прикладі додайте адресу електронної пошти генерального директора за мінімальною адресою.</span><span class="sxs-lookup"><span data-stu-id="14c78-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="14c78-114">**Додавання доменів для захисту**: додавання організаційної області, що включає в себе Office генерального директора.</span><span class="sxs-lookup"><span data-stu-id="14c78-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="14c78-115">**Виберіть дії**: **Якщо повідомлення електронної пошти надсилатиметься уособленним користувачем**, виберіть команду **перенаправити повідомлення до іншої адреси електронної пошти**, а потім введіть адресу електронної пошти адміністратора системи безпеки (наприклад, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="14c78-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="14c78-116">**Якщо повідомлення електронної пошти надсилатиметься уособленним доменом**, виберіть елемент **карантин**.</span><span class="sxs-lookup"><span data-stu-id="14c78-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="14c78-117">**Інтелект поштової скриньки**: за замовчуванням цей параметр вибирається під час створення нової анти-фішингової політики.</span><span class="sxs-lookup"><span data-stu-id="14c78-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="14c78-118">**Щоб отримати** кращі результати, залишіть цей параметр.</span><span class="sxs-lookup"><span data-stu-id="14c78-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="14c78-119">**Додавання надійних відправників і доменів:** У цьому прикладі не потрібно визначати всі зміни.</span><span class="sxs-lookup"><span data-stu-id="14c78-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="14c78-120">Переглянувши параметри, виберіть команду **створити цю політику** або **зберегти** відповідно.</span><span class="sxs-lookup"><span data-stu-id="14c78-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="14c78-121">Щоб отримати докладні відомості, ознайомтеся [з політикою захисту від фішингу в Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="14c78-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
