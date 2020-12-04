---
title: Виправлення неполадок із питанням ГВП
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573905"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="b0938-102">Виправлення неполадок із питанням ГВП</span><span class="sxs-lookup"><span data-stu-id="b0938-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="b0938-103">Для будь-якого пристрою, щоб завершити перевірку автентичності, вона має бути повністю авторизованим та в хорошому стані, а також отримати первинний маркер оновлення (PRT).</span><span class="sxs-lookup"><span data-stu-id="b0938-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="b0938-104">Під час реєстрації в гібридному полі Azure AD Реєстрація потрібні пристрої для корпоративної мережі.</span><span class="sxs-lookup"><span data-stu-id="b0938-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="b0938-105">Вона також працює над VPN, але є деякі застереження.</span><span class="sxs-lookup"><span data-stu-id="b0938-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="b0938-106">Ми почули клієнтів, які потребують допомоги з усунення несправностей, пов'язаних із процесом реєстрації в гібридному середовищі Azure.</span><span class="sxs-lookup"><span data-stu-id="b0938-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="b0938-107">Нижче наведено відомості про те, що відбувається під капотом під час реєстрації.</span><span class="sxs-lookup"><span data-stu-id="b0938-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="b0938-108">**Середовище автентифікації хмарного середовища (за допомогою синхронізації гешування пароля в Azure AD або передавання автентифікації)**</span><span class="sxs-lookup"><span data-stu-id="b0938-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="b0938-109">Цей потік реєстрації також відомий як "Sync JOIN".</span><span class="sxs-lookup"><span data-stu-id="b0938-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="b0938-110">Windows 10 виявляє запис SCP під час входу на пристрій.</span><span class="sxs-lookup"><span data-stu-id="b0938-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="b0938-111">Спочатку пристрій спробує отримати відомості про клієнта з надбудови "клієнт" у реєстрі [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="b0938-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="b0938-112">Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="b0938-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="b0938-113">Якщо це не вдасться, пристрій спілкується з локальною службою Active Directory (AD), щоб отримати відомості про клієнта з точки з'єднання служби (SCP).</span><span class="sxs-lookup"><span data-stu-id="b0938-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="b0938-114">Щоб перевірити програму SCP, зверніться до цього [документа](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="b0938-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="b0938-115">Ми рекомендуємо ввімкнути SCP в ОГОЛОШЕННІ та лише за допомогою клієнта SCP для початкової перевірки.</span><span class="sxs-lookup"><span data-stu-id="b0938-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="b0938-116">Операційна система Windows 10 намагається спілкуватися з Azure AD в контексті системи, щоб автентифікувати себе від Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0938-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="b0938-117">Ви можете перевірити, чи пристрій може отримати доступ до ресурсів Microsoft у системному обліковому записі за допомогою сценарію підключення випробувального пристрою.</span><span class="sxs-lookup"><span data-stu-id="b0938-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="b0938-118">Windows 10 створить сертифікат із власним підписом та зберігає його під об'єктом комп'ютера в локальній службі AD.</span><span class="sxs-lookup"><span data-stu-id="b0938-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="b0938-119">Для цього потрібно мати можливість прямої видимості для контролера домену.</span><span class="sxs-lookup"><span data-stu-id="b0938-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="b0938-120">Об'єкт пристрою, який має сертифікат, буде синхронізовано з Azure AD через Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b0938-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="b0938-121">Цикл синхронізації – кожні 30 хвилин за замовчуванням, але це залежить від конфігурації підключення Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0938-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="b0938-122">Щоб отримати докладніші відомості, зверніться до цього [документа](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="b0938-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="b0938-123">На цьому етапі ви зможете побачити тему пристрою в розділі "очікування" на пристрої з пристрою лазуровий портал.</span><span class="sxs-lookup"><span data-stu-id="b0938-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="b0938-124">Під час входу в обліковий запис до Windows 10 буде завершено реєстрацію.</span><span class="sxs-lookup"><span data-stu-id="b0938-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="b0938-125">Якщо ви працюєте в мережі VPN і не вдається ввійти в систему, ви можете ініціювати реєстрацію вручну.</span><span class="sxs-lookup"><span data-stu-id="b0938-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="b0938-126">Випуск dsregcmd/JOIN локально на панелі адміністратора або віддалено через smpexec на свій комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="b0938-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="b0938-127">Наприклад, Pssexec-s \\ win10client01 Cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="b0938-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="b0938-128">Докладні відомості про проблеми з гібридним об'єднанням наведено в статті [Виправлення неполадок із пристроями](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="b0938-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
