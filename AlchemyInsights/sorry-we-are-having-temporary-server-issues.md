---
title: Виправлення програм Microsoft 365 на жаль, у нас виникли проблеми з тимчасовими серверами
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758266"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="71224-102">Вирішення проблем із програмами Microsoft 365 "на жаль, повідомлення про тимчасові помилки сервера"</span><span class="sxs-lookup"><span data-stu-id="71224-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="71224-103">Якщо ви отримали це повідомлення, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="71224-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="71224-104">Перевірте брандмауер, антивірусне програмне забезпечення та параметри проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="71224-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="71224-105">Переглянути [діапазони URL-адрес і IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="71224-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="71224-106">Перейдіть на сторінку **Запуск**  >  **Run**, а потім введіть **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="71224-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="71224-107">Переконайтеся, що всі наведені нижче служби запущено.</span><span class="sxs-lookup"><span data-stu-id="71224-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="71224-108">Параметри автоматичного настроювання підключених мережних пристроїв</span><span class="sxs-lookup"><span data-stu-id="71224-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="71224-109">Служба "список мереж"</span><span class="sxs-lookup"><span data-stu-id="71224-109">Network List Service</span></span>
    - <span data-ttu-id="71224-110">Поінформованість про розташування мережі</span><span class="sxs-lookup"><span data-stu-id="71224-110">Network Location Awareness</span></span>
    - <span data-ttu-id="71224-111">Журнал подій Windows</span><span class="sxs-lookup"><span data-stu-id="71224-111">Windows Event Log</span></span>

<span data-ttu-id="71224-112">Якщо один із цих служб не запущено, випробуйте її, щоб почати.</span><span class="sxs-lookup"><span data-stu-id="71224-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="71224-113">Якщо у вас виникла проблема з запуском служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:</span><span class="sxs-lookup"><span data-stu-id="71224-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="71224-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="71224-114">**sfc /scannow**</span></span>

<span data-ttu-id="71224-115">Після завершення цієї команди перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="71224-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="71224-116">Докладні відомості наведено в статті ["на жаль, ми не можемо підключитися до вашого облікового запису. Спробуйте ще раз пізніше "помилка під час активації"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="71224-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>