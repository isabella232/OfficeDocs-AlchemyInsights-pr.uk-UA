---
title: Керування автоматичними оновленнями для програм Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439929"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="4405f-102">Керування автоматичними оновленнями для програм Office</span><span class="sxs-lookup"><span data-stu-id="4405f-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="4405f-103">За промовчанням оновлення для програм Office завантажуються автоматично та застосовуються у фоновому режимі без втручання користувача.</span><span class="sxs-lookup"><span data-stu-id="4405f-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="4405f-104">Проте адміністратори можуть контролювати, як оновлення застосовуються за допомогою настройок служби Office Update.</span><span class="sxs-lookup"><span data-stu-id="4405f-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="4405f-105">Параметри оновлення дають змогу адміністраторам вмикати й вимикати автоматичні оновлення, відображати або приховувати кнопку **оновити зараз** в Office, встановлювати терміни оновлення тощо.</span><span class="sxs-lookup"><span data-stu-id="4405f-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="4405f-106">Докладні відомості див.:</span><span class="sxs-lookup"><span data-stu-id="4405f-106">For detailed information, see:</span></span>

- [<span data-ttu-id="4405f-107">Настроювання параметрів оновлення для Office</span><span class="sxs-lookup"><span data-stu-id="4405f-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="4405f-108">Автоматичне оновлення для Office не ввімкнуто</span><span class="sxs-lookup"><span data-stu-id="4405f-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="4405f-109">Визначення способу оновлення Office після інсталяції</span><span class="sxs-lookup"><span data-stu-id="4405f-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="4405f-110">Щоб переглянути наявні настройки оновлень, застосовані до клієнтського комп'ютера, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="4405f-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="4405f-111">Відкрийте редактор **реєстру, перейшовши до запуску**  >  **Run**  >  **Regedit**.</span><span class="sxs-lookup"><span data-stu-id="4405f-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="4405f-112">Перейдіть до такого розташування та перегляньте параметри оновлення Office:</span><span class="sxs-lookup"><span data-stu-id="4405f-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="4405f-113">є.</span><span class="sxs-lookup"><span data-stu-id="4405f-113">a.</span></span> <span data-ttu-id="4405f-114">HKEY_LOCAL_MACHINE \ програмне Забезпечена\mice\офісr</span><span class="sxs-lookup"><span data-stu-id="4405f-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="4405f-115">B.</span><span class="sxs-lookup"><span data-stu-id="4405f-115">b.</span></span> <span data-ttu-id="4405f-116">Параметри залипання кнопки миші</span><span class="sxs-lookup"><span data-stu-id="4405f-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="4405f-117">**Зверніть увагу**  Якщо встановлено ключ officemgmtcom, може відображатися повідомлення "оновлення керуються системним адміністратором **" у**оновлення Office для  >  **облікового запису**Office  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="4405f-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="4405f-118">Для отримання додаткових відомостей див. [керування оновленнями для microsoft 365 програм за допомогою диспетчера конфігурацій Microsoft кінцевої точки](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="4405f-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  