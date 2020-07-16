---
title: Проблеми з відкриттям або завантаженням файлів у Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148439"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="dd4f7-102">Проблеми з відкриттям або завантаженням файлів у Yammer</span><span class="sxs-lookup"><span data-stu-id="dd4f7-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="dd4f7-103">Класична Yammer підтримує кілька варіантів завантаження файлів для повідомлень і груп.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="dd4f7-104">Залежно від конфігурації мережі, файли за замовчуванням для зберігання в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="dd4f7-105">Вибір файлів у новій Yammer ще не підтримує всі параметри, доступні в класичній Yammer.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="dd4f7-106">Майбутні оновлення будуть додавати додаткові функції.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-106">A future update will add additional features.</span></span> <span data-ttu-id="dd4f7-107">Для отримання додаткових відомостей див. [додайте файл або зображення до повідомлення про розмову Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="dd4f7-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="dd4f7-108">**Не вдається відкрити або завантажити файл**</span><span class="sxs-lookup"><span data-stu-id="dd4f7-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="dd4f7-109">Файл може бути вивантажене на Yammer, але також зв'язування з файлом у SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="dd4f7-110">Щоб усунути неполадки, спочатку потрібно визначити розташування файлу.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="dd4f7-111">Якщо файл завантажено до Yammer, він матиме URL-адресу \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="dd4f7-112">Переконайтеся, що потрібні URL-адреси та IP-адреси розблоковано.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="dd4f7-113">Для отримання додаткової інформації див у блозі [за допомогою жорстко кодованих IP-адрес для Yammer не рекомендується](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="dd4f7-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="dd4f7-114">Перевірте, чи користувач, який також є глобальним адміністратором, може завантажити файл.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="dd4f7-115">Якщо файл приватний, можливо, доведеться використовувати режим приватного вмісту.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="dd4f7-116">Для отримання додаткових відомостей [див.](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)</span><span class="sxs-lookup"><span data-stu-id="dd4f7-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="dd4f7-117">**Мережні гості та файли в SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="dd4f7-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="dd4f7-118">[Мережні гості Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не ВИКОРИСТОВУЮТЬ AZURE AD B2B і є внутрішніми для служби Yammer, тому вони не можуть отримати доступ до файлів Yammer, збережених у SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="dd4f7-119">Створення зовнішнього сад B2B користувача, який може отримати доступ до бібліотек документів SharePoint Online за допомогою цього посвідчення.</span><span class="sxs-lookup"><span data-stu-id="dd4f7-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="dd4f7-120">Відомості про майбутні Azure AD B2B підтримки гостя в Yammer, зверніться [до служби підтримки користувачів бізнес-бізнесу (B2B), у вікні попереднього перегляду Yammer та FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="dd4f7-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>