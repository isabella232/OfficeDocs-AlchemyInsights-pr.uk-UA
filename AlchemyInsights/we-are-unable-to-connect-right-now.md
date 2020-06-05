---
title: Активація питання-ми не вдалося підключитися зараз
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581896"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="748ee-102">Виправлення Microsoft 365 програм "ми не вдається підключитися зараз" повідомлення</span><span class="sxs-lookup"><span data-stu-id="748ee-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="748ee-103">Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="748ee-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="748ee-104">Перевірте настройки брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="748ee-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="748ee-105">Переглянути [URL-адреси Microsoft і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="748ee-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="748ee-106">Перейдіть до **запуску**  >  **Run**, а потім введіть **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="748ee-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="748ee-107">Переконайтеся, що виконуються такі служби:</span><span class="sxs-lookup"><span data-stu-id="748ee-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="748ee-108">Автоматичне настроювання мережних підключених пристроїв</span><span class="sxs-lookup"><span data-stu-id="748ee-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="748ee-109">Служба списку мереж</span><span class="sxs-lookup"><span data-stu-id="748ee-109">Network List Service</span></span>
    - <span data-ttu-id="748ee-110">Поінформованість про розташування в мережі</span><span class="sxs-lookup"><span data-stu-id="748ee-110">Network Location Awareness</span></span>
    - <span data-ttu-id="748ee-111">Журнал подій Windows</span><span class="sxs-lookup"><span data-stu-id="748ee-111">Windows Event Log</span></span>

<span data-ttu-id="748ee-112">Якщо одну з цих служб не запущено, спробуйте запустити його.</span><span class="sxs-lookup"><span data-stu-id="748ee-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="748ee-113">Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:</span><span class="sxs-lookup"><span data-stu-id="748ee-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="748ee-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="748ee-114">**sfc /scannow**</span></span>

<span data-ttu-id="748ee-115">Після завершення цієї команди, перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="748ee-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="748ee-116">Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації Office з Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="748ee-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>