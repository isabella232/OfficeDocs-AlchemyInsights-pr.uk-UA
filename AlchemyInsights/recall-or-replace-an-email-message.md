---
title: Відкликання або заміна повідомлення електронної пошти
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509477"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="4c6a3-102">Відкликання або заміна повідомлення електронної пошти в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4c6a3-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="4c6a3-103">Можна **відкликати лише повідомлення, надіслані людям у вашій організації**.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="4c6a3-104">Наприклад, якщо повідомлення надіслано на адресу Gmail, його не можна відкликати.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="4c6a3-105">Ви можете **відкликати лише повідомлення, надіслані з Outlook 2016 для ПК**.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="4c6a3-106">Якщо користувач надсилає повідомлення за допомогою Outlook для Mac або Outlook, в Інтернеті, ви не можете пригадати.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="4c6a3-107">Якщо ви адміністратор, ви можете **відкликати повідомлення від імені користувачів за допомогою PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="4c6a3-108">Повідомлення не можна відкликати з центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="4c6a3-109">Прокрутіть униз до пункту "Пошук і видалення повідомлень електронної пошти у вашій організації" для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="4c6a3-110">**Відкликання або замінювання повідомлення електронної пошти, надіслане**</span><span class="sxs-lookup"><span data-stu-id="4c6a3-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="4c6a3-111">В області папки зліва від вікна Outlook, виберіть надіслані папки.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="4c6a3-112">Відкрийте повідомлення, яке потрібно відкликати.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-112">Open the message that you want to recall.</span></span> <span data-ttu-id="4c6a3-113">Щоб відкрити повідомлення, потрібно двічі клацнути його.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-113">You must double-click to open the message.</span></span> <span data-ttu-id="4c6a3-114">Якщо вибрати повідомлення, яке воно відображається в області читання, не дозволить відкликати повідомлення.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="4c6a3-115">На вкладці повідомлення виберіть дії, **Actions**  >  **відкликання цього повідомлення**.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="4c6a3-116">Виберіть **Видалити непрочитані копії цього повідомлення** або **Видалити непрочитані копії та замінити новим повідомленням**, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="4c6a3-117">Якщо ви надсилаєте повідомлення про заміну, складіть повідомлення та натисніть **Надіслати**.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="4c6a3-118">Успішність або невдача відкликання повідомлення залежить від параметрів одержувачів у Outlook.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="4c6a3-119">Для отримання додаткових відомостей, зокрема про те, як [перевірити відкликання, див.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="4c6a3-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="4c6a3-120">***Пошук і видалення повідомлень електронної пошти в організації*** Щоб знайти та видалити повідомлення електронної пошти в організації, простіше, якщо ви Глобальний адміністратор. Якщо ви не є глобальним адміністратором, потрібно додати обліковий запис до рольової групи "Диспетчер Витребування" або до ролі керування пошуком відповідності.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="4c6a3-121">Щоб видалити повідомлення, потрібно приєднатися до рольової групи «керування організацією» або ролі керування пошуком і очищення.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="4c6a3-122">Дозволи на доступ до цих ролей призначаються у [центрі дотримання правил безпеки &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="4c6a3-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="4c6a3-123">[Створіть пошук вмісту](https://docs.microsoft.com/microsoft-365/compliance/content-search) , щоб знайти повідомлення для видалення.</span><span class="sxs-lookup"><span data-stu-id="4c6a3-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="4c6a3-124">[Підключення до безпеки & центр відповідності PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="4c6a3-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="4c6a3-125">Якщо ви використовуєте МЗС, див. [підключитися до Microsoft 365 безпеки & центр відповідності PowerShell, використовуючи автентифікацію на кількох факторів](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="4c6a3-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
