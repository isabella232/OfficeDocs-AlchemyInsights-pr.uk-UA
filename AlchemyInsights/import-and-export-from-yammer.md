---
title: Імпорт і експорт з Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037254"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="44d98-102">Імпорт і експорт з Yammer</span><span class="sxs-lookup"><span data-stu-id="44d98-102">Import and export from Yammer</span></span>

<span data-ttu-id="44d98-103">**Імпорт**</span><span class="sxs-lookup"><span data-stu-id="44d98-103">**Import**</span></span>

<span data-ttu-id="44d98-104">Варіанти імпорту користувача залежать від того, чи мережа Yammer працює в [рідному режимі для Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)або ні.</span><span class="sxs-lookup"><span data-stu-id="44d98-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="44d98-105">**Нерідний режим**: користувачі можуть імпортувати їх до груп за допомогою [Додавання з адресної книги](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (обмеження до 100 користувачів) в межах групи або в мережі за допомогою [групового оновлення](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) в межах мережі.</span><span class="sxs-lookup"><span data-stu-id="44d98-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="44d98-106">**Рідний режим**: операції з членством у групах і членство в мережі мають виконуватися на [порталі адміністрування Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), порталу " [Лазурний](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)" або за допомогою іншого параметра Azure AD.</span><span class="sxs-lookup"><span data-stu-id="44d98-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="44d98-107">Мережі в рідному режимі більше не мають доступу до групового оновлення та інших застарілих функцій.</span><span class="sxs-lookup"><span data-stu-id="44d98-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="44d98-108">Yammer ніколи не підтримував імпорт вмісту з адміністратора мережі, навіть коли в іншій мережі використовувався функція експорту даних.</span><span class="sxs-lookup"><span data-stu-id="44d98-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="44d98-109">Вміст може бути повторно надіслано партнерськими рішеннями або API REST Yammer.</span><span class="sxs-lookup"><span data-stu-id="44d98-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="44d98-110">**Експорт**</span><span class="sxs-lookup"><span data-stu-id="44d98-110">**Export**</span></span>

<span data-ttu-id="44d98-111">[Експорт даних мережі в межах адміністратора мережі](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) дає можливість експортувати вміст у мережі Yammer, зокрема про повідомлення та файли.</span><span class="sxs-lookup"><span data-stu-id="44d98-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="44d98-112">Вкладення можуть бути надзвичайно великими, і це призведе до того, що експорт матиме значний час для виконання.</span><span class="sxs-lookup"><span data-stu-id="44d98-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="44d98-113">Ми рекомендуємо активувати активні мережі за допомогою [API експорту даних](https://developer.yammer.com/docs/data-export-api) на шматки за день або тиждень.</span><span class="sxs-lookup"><span data-stu-id="44d98-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="44d98-114">Служба підтримки Microsoft не надає спеціальні сценарії для цієї мети.</span><span class="sxs-lookup"><span data-stu-id="44d98-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="44d98-115">Для експорту вмісту для окремого користувача існує окремий [експорт Гдпр](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) .</span><span class="sxs-lookup"><span data-stu-id="44d98-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>