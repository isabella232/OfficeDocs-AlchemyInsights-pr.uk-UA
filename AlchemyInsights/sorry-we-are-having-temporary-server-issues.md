---
title: Виправлення Microsoft 365 Apps Вибачте, у нас виникли тимчасові проблеми з сервером повідомлення
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582724"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="98f30-102">Виправлення Microsoft 365 Apps "Вибачте, ми виникли проблеми з тимчасового сервера"</span><span class="sxs-lookup"><span data-stu-id="98f30-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="98f30-103">Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="98f30-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="98f30-104">Перевірте настройки брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="98f30-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="98f30-105">Перегляд [URL-адрес і діапазонів IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="98f30-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="98f30-106">Перейдіть до **запуску**  >  **Run**, а потім введіть **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="98f30-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="98f30-107">Переконайтеся, що виконуються такі служби:</span><span class="sxs-lookup"><span data-stu-id="98f30-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="98f30-108">Автоматичне настроювання мережних підключених пристроїв</span><span class="sxs-lookup"><span data-stu-id="98f30-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="98f30-109">Служба списку мереж</span><span class="sxs-lookup"><span data-stu-id="98f30-109">Network List Service</span></span>
    - <span data-ttu-id="98f30-110">Поінформованість про розташування в мережі</span><span class="sxs-lookup"><span data-stu-id="98f30-110">Network Location Awareness</span></span>
    - <span data-ttu-id="98f30-111">Журнал подій Windows</span><span class="sxs-lookup"><span data-stu-id="98f30-111">Windows Event Log</span></span>

<span data-ttu-id="98f30-112">Якщо одну з цих служб не запущено, спробуйте запустити його.</span><span class="sxs-lookup"><span data-stu-id="98f30-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="98f30-113">Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:</span><span class="sxs-lookup"><span data-stu-id="98f30-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="98f30-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="98f30-114">**sfc /scannow**</span></span>

<span data-ttu-id="98f30-115">Після завершення цієї команди, перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="98f30-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="98f30-116">Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="98f30-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>