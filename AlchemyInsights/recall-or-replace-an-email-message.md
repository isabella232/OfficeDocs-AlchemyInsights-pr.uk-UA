---
title: Відкликання або заміна повідомлення електронної пошти
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353527"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="540e7-102">Відкликання або заміна повідомлення електронної пошти в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="540e7-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="540e7-103">Ви можете **згадати лише повідомлення, надіслані користувачам вашої організації**.</span><span class="sxs-lookup"><span data-stu-id="540e7-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="540e7-104">Наприклад, якщо повідомлення надіслано на адресу Gmail, його не можна пригадати.</span><span class="sxs-lookup"><span data-stu-id="540e7-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="540e7-105">Ви можете **відкликати повідомлення, надіслані з програми Outlook для ПК**.</span><span class="sxs-lookup"><span data-stu-id="540e7-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="540e7-106">Якщо користувач надсилає повідомлення за допомогою програми Outlook для Mac або Інтернет-версії Outlook, ви не можете пригадати її.</span><span class="sxs-lookup"><span data-stu-id="540e7-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="540e7-107">Як адміністратор клієнта ви можете **відкликати повідомлення від імені користувачів за допомогою PowerShell** (для отримання додаткових відомостей див. в статті [Пошук і видалення повідомлень електронної пошти](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="540e7-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="540e7-108">Ви не можете відкликати повідомлення з центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="540e7-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="540e7-109">Прокрутіть униз до розділу "Пошук і видалення повідомлень електронної пошти в організації", щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="540e7-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="540e7-110">**Відкликання або заміна повідомлення електронної пошти, яке ви надіслали**</span><span class="sxs-lookup"><span data-stu-id="540e7-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="540e7-111">В області папок ліворуч у вікні програми Outlook виберіть папку Надіслані.</span><span class="sxs-lookup"><span data-stu-id="540e7-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="540e7-112">Відкрийте повідомлення, яке потрібно відкликати.</span><span class="sxs-lookup"><span data-stu-id="540e7-112">Open the message that you want to recall.</span></span> <span data-ttu-id="540e7-113">Щоб відкрити повідомлення, потрібно двічі клацнути його.</span><span class="sxs-lookup"><span data-stu-id="540e7-113">You must double-click to open the message.</span></span> <span data-ttu-id="540e7-114">Виділення повідомлення, яке відображається в області читання, не дасть змогу відкликати повідомлення.</span><span class="sxs-lookup"><span data-stu-id="540e7-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="540e7-115">На вкладці повідомлення установіть прапорець **дії**, щоб  >  **відкликати це повідомлення**.</span><span class="sxs-lookup"><span data-stu-id="540e7-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="540e7-116">Виберіть команду **Видалити непрочитані копії цього повідомлення** або **Видалити непрочитані копії та замінити на нове повідомлення**, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="540e7-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="540e7-117">Якщо ви надсилаєте повідомлення про заміну, створіть повідомлення, а потім натисніть кнопку **Надіслати**.</span><span class="sxs-lookup"><span data-stu-id="540e7-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="540e7-118">Успіх або відмова від відкликання повідомлення залежить від параметрів одержувачів у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="540e7-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="540e7-119">Додаткові відомості, зокрема про те, як перевірити відкликання, наведено в статті [відкликання або замінення повідомлення електронної пошти, яке ви надіслали](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="540e7-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="540e7-120">**_Для пошуку та видалення повідомлень електронної пошти в організації_** простіше, якщо ви – Глобальний адміністратор. Якщо ви не є глобальним адміністратором, ваш обліковий запис має бути додано до рольової групи "Диспетчер Витребування" або до ролі керування пошуком відповідності.</span><span class="sxs-lookup"><span data-stu-id="540e7-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="540e7-121">Щоб видалити повідомлення, потрібно приєднатися до рольової групи "Керування організацією" або "Пошук і очищення".</span><span class="sxs-lookup"><span data-stu-id="540e7-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="540e7-122">Дозволи для цих ролей призначено в [центрі відповідності & безпеки](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="540e7-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="540e7-123">[Створіть пошук вмісту](https://docs.microsoft.com/microsoft-365/compliance/content-search) , щоб знайти повідомлення, яке потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="540e7-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="540e7-124">[Підключення до центру безпеки та відповідності & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="540e7-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="540e7-125">Якщо ви використовуєте програму МЗС (багатофакторна автентифікація), перегляньте статтю [підключитися до служби безпеки Microsoft 365 & центр відповідності PowerShell за допомогою багатофакторної автентифікації](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="540e7-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
