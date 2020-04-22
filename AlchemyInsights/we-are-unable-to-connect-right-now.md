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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716193"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="277b4-102">Виправлення програми Office "не вдається підключитися зараз" повідомлення</span><span class="sxs-lookup"><span data-stu-id="277b4-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="277b4-103">Якщо з'являється це повідомлення, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="277b4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="277b4-104">Перевірте брандмауер, антивірусне програмне забезпечення та настройки проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Office.</span><span class="sxs-lookup"><span data-stu-id="277b4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="277b4-105">Переглянути [URL-адреси Microsoft і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="277b4-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="277b4-106">Перейдіть до **запуску** > **, а**потім введіть **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="277b4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="277b4-107">Переконайтеся, що виконуються такі служби:</span><span class="sxs-lookup"><span data-stu-id="277b4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="277b4-108">Автоматичне настроювання мережних підключених пристроїв</span><span class="sxs-lookup"><span data-stu-id="277b4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="277b4-109">Служба списку мереж</span><span class="sxs-lookup"><span data-stu-id="277b4-109">Network List Service</span></span>
    - <span data-ttu-id="277b4-110">Поінформованість про розташування в мережі</span><span class="sxs-lookup"><span data-stu-id="277b4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="277b4-111">Журнал подій Windows</span><span class="sxs-lookup"><span data-stu-id="277b4-111">Windows Event Log</span></span>

<span data-ttu-id="277b4-112">Якщо одну з цих служб не запущено, спробуйте запустити його.</span><span class="sxs-lookup"><span data-stu-id="277b4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="277b4-113">Якщо проблема запуску служби, виконайте таку команду, відкривши командний рядок із підвищеними дозволами:</span><span class="sxs-lookup"><span data-stu-id="277b4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="277b4-114">**SFC/SCANNOW**</span><span class="sxs-lookup"><span data-stu-id="277b4-114">**sfc /scannow**</span></span>

<span data-ttu-id="277b4-115">Після завершення цієї команди, перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="277b4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="277b4-116">Докладні відомості наведено [в "Вибачте, ми не можемо підключитися до вашого облікового запису. Повторіть спробу пізніше "помилка під час активації Office з Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="277b4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>