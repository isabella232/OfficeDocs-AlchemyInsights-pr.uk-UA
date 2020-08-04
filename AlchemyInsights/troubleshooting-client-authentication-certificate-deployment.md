---
title: Виправлення неполадок розгортання сертифіката автентифікації клієнта
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555805"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="76c06-102">Виправлення неполадок розгортання сертифіката автентифікації клієнта</span><span class="sxs-lookup"><span data-stu-id="76c06-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="76c06-103">InTune та PKCS/PFX профілі клієнтських сертифікатів зазвичай використовуються в поєднанні з іншими типами профілів, такими як WiFi, VPN і електронна пошта, щоб дозволити користувачам автентифікувати корпоративні ресурси.</span><span class="sxs-lookup"><span data-stu-id="76c06-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="76c06-104">Під час цих типів профілів, пов'язані з профілю клієнтський сертифікат залежить від успішного розгортання цього профілю.</span><span class="sxs-lookup"><span data-stu-id="76c06-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="76c06-105">Початкова настройка інфраструктури та пов'язана конфігурація профілю клієнтського сертифіката часто потребують виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="76c06-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="76c06-106">Покрокові інструкції з успішної інсталяції з'єднувач NDES і інструкції з виправлення неполадок, щоб виділити проблеми з розгортання сертифікатів див.:</span><span class="sxs-lookup"><span data-stu-id="76c06-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="76c06-107">Настроювання інфраструктури для підтримки SCEP з InTune</span><span class="sxs-lookup"><span data-stu-id="76c06-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="76c06-108">Огляд для виправлення неполадок SCEP, сертифікати з Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="76c06-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="76c06-109">Використовуйте посилання PowerShell сценаріїв, які допоможуть перевірити конфігурацію.</span><span class="sxs-lookup"><span data-stu-id="76c06-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="76c06-110">Для отримання додаткових [відомостей див.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)</span><span class="sxs-lookup"><span data-stu-id="76c06-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="76c06-111">**Інші поширені проблеми**</span><span class="sxs-lookup"><span data-stu-id="76c06-111">**Other common issues**</span></span>

<span data-ttu-id="76c06-112">**Під час спроби інсталювати з'єднувач сертифіката InTune на сервері з'єднувача NDES, я отримую повідомлення "пароль у запиті сертифіката не можна перевірити. Можливо, це вже було використане. Отримати новий пароль для надсилання з цим запитом. "**</span><span class="sxs-lookup"><span data-stu-id="76c06-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="76c06-113">Це повідомлення означає, що потрібно запустити інсталяцію з'єднувач сертифікатів із правами адміністратора.</span><span class="sxs-lookup"><span data-stu-id="76c06-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="76c06-114">У деяких середовищах сервери, де запущено InTune сертифікат має використовувати проксі-сервер для підключення до InTune, і тому з'єднувач сертифікат має використовувати проксі-сервер.</span><span class="sxs-lookup"><span data-stu-id="76c06-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="76c06-115">У деяких випадках з'єднувач NDES ігнорує налаштовані настройки проксі-сервера, і може бути необхідно настроїти параметри проксі-сервера під час роботи в контексті безпеки LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="76c06-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="76c06-116">Рішення полягає в тому, щоб запустити Internet Explorer як СИСТЕМУ і налаштувати проксі в IE.</span><span class="sxs-lookup"><span data-stu-id="76c06-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="76c06-117">Після перезапуску служби InTune з'єднувача, з'єднувач NDES підключається до InTune.</span><span class="sxs-lookup"><span data-stu-id="76c06-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="76c06-118">**Пристрої користувача більше не отримують сертифікати SCEP від NDES.**</span><span class="sxs-lookup"><span data-stu-id="76c06-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="76c06-119">Можливо, сертифікат автентифікації клієнта, виданий на сервері NDES, і вказаний під час інсталяції з'єднувача NDES, минув або відсутній.</span><span class="sxs-lookup"><span data-stu-id="76c06-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="76c06-120">Щоб вирішити проблему:</span><span class="sxs-lookup"><span data-stu-id="76c06-120">To resolve:</span></span> 
 
1. <span data-ttu-id="76c06-121">Видаліть з'єднувач NDES.</span><span class="sxs-lookup"><span data-stu-id="76c06-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="76c06-122">Використовуйте ці відомості для запиту автентифікації клієнта або сертифіката автентифікації сервера:</span><span class="sxs-lookup"><span data-stu-id="76c06-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="76c06-123">Тема Назва: CN = зовнішнє доменне ім'я</span><span class="sxs-lookup"><span data-stu-id="76c06-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="76c06-124">Тема альтернативне ім'я (обидва обов'язкові): DNS = зовнішнє FQDN, DNS = внутрішнє ім'я FQDN</span><span class="sxs-lookup"><span data-stu-id="76c06-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="76c06-125">Переінсталюйте з'єднувач NDES з новим сертифікатом.</span><span class="sxs-lookup"><span data-stu-id="76c06-125">Reinstall the NDES connector with the new certificate.</span></span>