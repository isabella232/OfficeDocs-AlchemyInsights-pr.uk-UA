---
title: Відкликання або заміна повідомлення електронної пошти в Outlook для настільних комп'ютерів
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664011"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="8f013-102">Відкликання або заміна повідомлення електронної пошти Outlook</span><span class="sxs-lookup"><span data-stu-id="8f013-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="8f013-103">Адміністратор може **відкликати повідомлення від імені користувачів за допомогою PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="8f013-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="8f013-104">Ви не можете відкликати повідомлення з центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="8f013-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="8f013-105">Ви можете **згадати лише повідомлення, надіслані користувачам вашої організації**.</span><span class="sxs-lookup"><span data-stu-id="8f013-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="8f013-106">Якщо повідомлення надіслано на адресу Gmail, наприклад, ви не можете пригадати її.</span><span class="sxs-lookup"><span data-stu-id="8f013-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="8f013-107">Ви можете **відкликати повідомлення, надіслані з Outlook 2016 на ПК**.</span><span class="sxs-lookup"><span data-stu-id="8f013-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="8f013-108">Якщо користувач надсилає повідомлення за допомогою програми Outlook для Mac або Інтернет-версії Outlook, ви не можете пригадати її.</span><span class="sxs-lookup"><span data-stu-id="8f013-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="8f013-109">Щоб відкликати або замінити повідомлення електронної пошти, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="8f013-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="8f013-110">В області папок ліворуч у вікні програми Outlook виберіть папку Надіслані.</span><span class="sxs-lookup"><span data-stu-id="8f013-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="8f013-111">Двічі клацніть повідомлення, яке потрібно згадати, щоб відкрити його.</span><span class="sxs-lookup"><span data-stu-id="8f013-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="8f013-112">Перейдіть на вкладку **повідомлення** , а потім виберіть **дії**, щоб  >  **відкликати це повідомлення**.</span><span class="sxs-lookup"><span data-stu-id="8f013-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="8f013-113">Виберіть команду **Видалити непрочитані копії цього повідомлення** або **Видалити непрочитані копії та замінити на нове повідомлення**, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="8f013-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="8f013-114">Якщо ви надсилаєте повідомлення про заміну, напишіть повідомлення та натисніть кнопку **Надіслати**.</span><span class="sxs-lookup"><span data-stu-id="8f013-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="8f013-115">Успіх або відмова від відкликання повідомлення залежить від параметрів одержувача в програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="8f013-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="8f013-116">Щоб отримати вказівки з відкликання, ознайомтеся з [цією статтею](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="8f013-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="8f013-117">Пошук і видалення повідомлень електронної пошти в організації</span><span class="sxs-lookup"><span data-stu-id="8f013-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="8f013-118">Якщо ви не є глобальним адміністратором, ваш обліковий запис має бути додано до ролі диспетчера Витребування електронної інформації або роль керування пошуком за відповідність для пошуку повідомлень.</span><span class="sxs-lookup"><span data-stu-id="8f013-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="8f013-119">Щоб видалити повідомлення, потрібно приєднатися до рольової групи "Керування організацією" або "Пошук і очищення".</span><span class="sxs-lookup"><span data-stu-id="8f013-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="8f013-120">Дозволи для цих ролей призначено в [центрі безпеки та відповідності](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="8f013-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="8f013-121">[Створіть пошук вмісту](https://docs.microsoft.com/microsoft-365/compliance/content-search) , щоб знайти повідомлення, яке потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="8f013-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="8f013-122">[Підключення до центру безпеки та відповідності PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="8f013-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="8f013-123">Якщо використовується багатофакторна автентифікація, перегляньте статтю [підключитися до центру безпеки та відповідності Microsoft 365 за допомогою багатофакторної автентифікації](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="8f013-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>