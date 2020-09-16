---
title: Виправлення неполадок розгортання сертифіката автентифікації клієнта
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659007"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="4dd32-102">Виправлення неполадок розгортання сертифіката автентифікації клієнта</span><span class="sxs-lookup"><span data-stu-id="4dd32-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="4dd32-103">Для користувачів, які використовують інші типи профілів, як-от Wi-Fi, VPN і електронна пошта, можна дозволити користувачам автентифікувати корпоративні ресурси.</span><span class="sxs-lookup"><span data-stu-id="4dd32-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="4dd32-104">Якщо ці типи профілів зв'язані з профілем сертифіката клієнта, залежить від успішного розгортання цього профілю.</span><span class="sxs-lookup"><span data-stu-id="4dd32-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="4dd32-105">Початкова настройка інфраструктури та відповідна конфігурація профілю сертифіката клієнта часто вимагають виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="4dd32-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="4dd32-106">Щоб отримати покрокові вказівки з успішної інсталяції сполучної лінії NDES і рекомендації з виправлення неполадок, щоб ізолювати проблеми з розгортанням сертифіката, див.:</span><span class="sxs-lookup"><span data-stu-id="4dd32-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="4dd32-107">Настроювання інфраструктури для підтримки функції SCEP з Inune</span><span class="sxs-lookup"><span data-stu-id="4dd32-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="4dd32-108">Огляд виправлення неполадок із профілях сертифікатів SCEP за допомогою Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="4dd32-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="4dd32-109">Щоб перевірити конфігурацію, використовуйте посилання на сценарії PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4dd32-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="4dd32-110">Щоб отримати докладні відомості, перегляньте [сценарії перевірки сполучної лінії сертифіката "Inune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)".</span><span class="sxs-lookup"><span data-stu-id="4dd32-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="4dd32-111">**Інші поширені проблеми**</span><span class="sxs-lookup"><span data-stu-id="4dd32-111">**Other common issues**</span></span>

<span data-ttu-id="4dd32-112">**Під час спроби інсталювати з'єднувач сертифіката Inune на сервері з'єднувача NDES відображається повідомлення "пароль у запиті сертифіката не можна перевірити. Можливо, він уже використовувався. Отримайте новий пароль, щоб надіслати цей запит. "**</span><span class="sxs-lookup"><span data-stu-id="4dd32-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="4dd32-113">Це повідомлення означає, що потрібно запустити інсталяцію з'єднувача сертифіката як адміністратор.</span><span class="sxs-lookup"><span data-stu-id="4dd32-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="4dd32-114">У деяких середовищах сервера, на якому запущено сертифікат Inune, має використовувати проксі-сервер для підключення до веб-сервера, і тому з'єднувач сертифіката має використовувати проксі.</span><span class="sxs-lookup"><span data-stu-id="4dd32-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="4dd32-115">За певних обставин сполучна лінія NDES ігнорує настроєні параметри проксі-сервера, і, можливо, знадобиться настроїти параметри проксі-сервера під час роботи в контексті безпеки LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="4dd32-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="4dd32-116">Рішення – запустити Internet Explorer як СИСТЕМУ та настроїти проксі-сервер у IE.</span><span class="sxs-lookup"><span data-stu-id="4dd32-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="4dd32-117">Після перезапуску служби з'єднувача Inune, сполучна лінія NDES підключається до веб-програми Inune.</span><span class="sxs-lookup"><span data-stu-id="4dd32-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="4dd32-118">**Пристрої користувача більше не отримують сертифікатів SCEP від NDES.**</span><span class="sxs-lookup"><span data-stu-id="4dd32-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="4dd32-119">Можливо, сертифікат автентифікації клієнта, виданий на сервері NDES, і вказаний під час інсталяції з'єднувача NDES, минув або відсутній.</span><span class="sxs-lookup"><span data-stu-id="4dd32-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="4dd32-120">Щоб вирішити, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="4dd32-120">To resolve:</span></span> 
 
1. <span data-ttu-id="4dd32-121">Видаліть сполучну лінію NDES.</span><span class="sxs-lookup"><span data-stu-id="4dd32-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="4dd32-122">Щоб надіслати запит на отримання нової автентифікації клієнта або сертифіката автентифікації на сервері, виконайте наведені нижче відомості.</span><span class="sxs-lookup"><span data-stu-id="4dd32-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="4dd32-123">Ім'я суб'єкта: CN = зовнішній FQDN</span><span class="sxs-lookup"><span data-stu-id="4dd32-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="4dd32-124">Назва альтернативної теми (для обох обов'язкових): DNS = зовнішній FQDN, DNS = внутрішній FQDN</span><span class="sxs-lookup"><span data-stu-id="4dd32-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="4dd32-125">Повторно інсталюйте сполучну лінію NDES, використовуючи новий сертифікат.</span><span class="sxs-lookup"><span data-stu-id="4dd32-125">Reinstall the NDES connector with the new certificate.</span></span>