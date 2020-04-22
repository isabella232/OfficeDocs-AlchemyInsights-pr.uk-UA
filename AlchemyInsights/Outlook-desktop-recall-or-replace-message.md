---
title: Outlook для робочого столу відкликати або замінити повідомлення електронної пошти
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687531"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="2c102-102">Відкликання або заміна повідомлення електронної пошти Outlook</span><span class="sxs-lookup"><span data-stu-id="2c102-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="2c102-103">Як адміністратор, ви можете **відкликати повідомлення від імені користувачів за допомогою PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="2c102-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="2c102-104">Повідомлення не можна відкликати з центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="2c102-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="2c102-105">Можна **відкликати лише повідомлення, надіслані людям у вашій організації**.</span><span class="sxs-lookup"><span data-stu-id="2c102-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="2c102-106">Наприклад, якщо повідомлення надіслано на адресу Gmail, його не можна відкликати.</span><span class="sxs-lookup"><span data-stu-id="2c102-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="2c102-107">Ви можете **відкликати лише повідомлення, надіслані з Outlook 2016 на ПК**.</span><span class="sxs-lookup"><span data-stu-id="2c102-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="2c102-108">Якщо користувач надсилає повідомлення за допомогою Outlook для Mac або Outlook, в Інтернеті, ви не можете пригадати.</span><span class="sxs-lookup"><span data-stu-id="2c102-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="2c102-109">Щоб відкликати або замінити повідомлення електронної пошти:</span><span class="sxs-lookup"><span data-stu-id="2c102-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="2c102-110">В області папки зліва від вікна Outlook, виберіть надіслані папки.</span><span class="sxs-lookup"><span data-stu-id="2c102-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="2c102-111">Двічі клацніть повідомлення, яке потрібно відкликати, щоб відкрити його.</span><span class="sxs-lookup"><span data-stu-id="2c102-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="2c102-112">Перейдіть на вкладку **повідомлення** , а потім виберіть **дії** > , які**відкликають це повідомлення**.</span><span class="sxs-lookup"><span data-stu-id="2c102-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="2c102-113">Виберіть **Видалити непрочитані копії повідомлення** або **Видалити непрочитані копії та замінити новим повідомленням**, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="2c102-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="2c102-114">Якщо ви надсилаєте повідомлення про заміну, складете повідомлення, а потім виберіть **Надіслати**.</span><span class="sxs-lookup"><span data-stu-id="2c102-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="2c102-115">Успішність або невдача відкликання повідомлення залежить від параметрів одержувача в Outlook.</span><span class="sxs-lookup"><span data-stu-id="2c102-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="2c102-116">Для кроків, щоб перевірити на відкликання, див [у цій статті](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="2c102-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="2c102-117">Пошук і видалення повідомлень електронної пошти в організації</span><span class="sxs-lookup"><span data-stu-id="2c102-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="2c102-118">Якщо ви не є глобальним адміністратором, ваш обліковий запис потрібно додати до ролі диспетчера Витребування або виконання ролей керування пошуком для пошуку повідомлень.</span><span class="sxs-lookup"><span data-stu-id="2c102-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="2c102-119">Щоб видалити повідомлення, потрібно приєднатися до рольової групи «керування організацією» або ролі керування пошуком і очищення.</span><span class="sxs-lookup"><span data-stu-id="2c102-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="2c102-120">Дозволи для цих ролей призначаються в [центрі безпеки та комплаєнсу](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="2c102-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="2c102-121">[Створіть пошук вмісту](https://docs.microsoft.com/office365/securitycompliance/content-search) , щоб знайти повідомлення для видалення.</span><span class="sxs-lookup"><span data-stu-id="2c102-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="2c102-122">[Підключення до центру безпеки та комплаєнсу PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2c102-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="2c102-123">Якщо використовується багатофакторна автентифікація, див., [підключення до Microsoft 365 безпеки та дотримання центру PowerShell, використовуючи автентифікацію на кількох факторів](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2c102-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>