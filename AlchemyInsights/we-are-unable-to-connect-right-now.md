---
title: Проблема з активацією – не вдалося підключитися зараз
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806463"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="878e7-102">Виправлення помилок у програмах Microsoft 365 "Не вдалося підключитися зараз"</span><span class="sxs-lookup"><span data-stu-id="878e7-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="878e7-103">Якщо ви отримали це повідомлення, спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="878e7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="878e7-104">Перевірте параметри брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ до Інтернету до програм Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="878e7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="878e7-105">Докладні [відомості див. в статті Діапазони URL- і IP-адрес Корпорації Майкрософт.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="878e7-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="878e7-106">Відкрийте меню **"Пуск"**  >  і введіть **services.msc.**</span><span class="sxs-lookup"><span data-stu-id="878e7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="878e7-107">Переконайтеся, що всі ці служби запущено:</span><span class="sxs-lookup"><span data-stu-id="878e7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="878e7-108">Автоматичне настроювання підключених мережевих пристроїв</span><span class="sxs-lookup"><span data-stu-id="878e7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="878e7-109">Служба списку мережі</span><span class="sxs-lookup"><span data-stu-id="878e7-109">Network List Service</span></span>
    - <span data-ttu-id="878e7-110">Усвідомлення мережевого розташування</span><span class="sxs-lookup"><span data-stu-id="878e7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="878e7-111">Журнал подій Windows</span><span class="sxs-lookup"><span data-stu-id="878e7-111">Windows Event Log</span></span>

<span data-ttu-id="878e7-112">Якщо одну з цих служб не запущено, спробуйте запустити її.</span><span class="sxs-lookup"><span data-stu-id="878e7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="878e7-113">Якщо під час запуску служби відобразиться помилка, запустіть наведену нижче команду, відкривши командний рядок із дозволами в режимі адміністратора.</span><span class="sxs-lookup"><span data-stu-id="878e7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="878e7-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="878e7-114">**sfc /scannow**</span></span>

<span data-ttu-id="878e7-115">Коли ця команда завершиться, перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="878e7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="878e7-116">Докладні відомості див. в [розділі "На жаль, не вдалося підключитися до вашого облікового запису. Спробуйте ще раз пізніше" під час активації Office зі служби Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="878e7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>