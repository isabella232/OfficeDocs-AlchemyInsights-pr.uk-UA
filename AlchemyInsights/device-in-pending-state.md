---
title: Пристрій у стані очікування
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679996"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="9cd87-102">Пристрій у стані очікування</span><span class="sxs-lookup"><span data-stu-id="9cd87-102">Device in pending state</span></span>

<span data-ttu-id="9cd87-103">**Попередні вимоги**</span><span class="sxs-lookup"><span data-stu-id="9cd87-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="9cd87-104">Якщо ви вперше налаштували реєстрації пристрою, переконайтеся, що ви переглянули [Загальні відомості про керування пристроями в Лазурому Active Directory (ЛАЗУРНЕ AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , що допоможе вам отримати доступ до пристроїв під елементом керування Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9cd87-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="9cd87-105">Якщо ви реєструєте пристрої в Azure AD безпосередньо та вступивши їх у програму Inune, потрібно переконатися, що ви [настроїли](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) програму та маєте [ліцензію](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) на перше місце.</span><span class="sxs-lookup"><span data-stu-id="9cd87-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="9cd87-106">Переконайтеся, що ви маєте право виконувати операції в Лазурому та локальному ОГОЛОШЕННІ.</span><span class="sxs-lookup"><span data-stu-id="9cd87-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="9cd87-107">Параметри для реєстрації пристроїв можна керувати лише глобальним адміністратором в Лазур AD.</span><span class="sxs-lookup"><span data-stu-id="9cd87-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="9cd87-108">Крім того, якщо ви настроїли автоматичну реєстрацію в локальній службі Active Directory, вам потрібно бути адміністратором служби Active Directory та AD FS (якщо це можливо).</span><span class="sxs-lookup"><span data-stu-id="9cd87-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="9cd87-109">Для гібридного процесу реєстрації в процесі об'єднання лазуровий, потрібні пристрої для корпоративної мережі.</span><span class="sxs-lookup"><span data-stu-id="9cd87-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="9cd87-110">Вона також працює над VPN, але є деякі застереження.</span><span class="sxs-lookup"><span data-stu-id="9cd87-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="9cd87-111">Ми почули клієнтів, які потребують допомоги з усунення несправностей, пов'язаних із процесом реєстрації в гібридному полі Azure, за умовами віддалених робочих умов.</span><span class="sxs-lookup"><span data-stu-id="9cd87-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="9cd87-112">**Середовище автентифікації хмарного середовища (за допомогою синхронізації гешування пароля в Azure AD або передавання автентифікації)**</span><span class="sxs-lookup"><span data-stu-id="9cd87-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="9cd87-113">Цей потік реєстрації також відомий як "Sync JOIN".</span><span class="sxs-lookup"><span data-stu-id="9cd87-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="9cd87-114">Нижче наведено відомості про те, що відбувається під час реєстрації.</span><span class="sxs-lookup"><span data-stu-id="9cd87-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="9cd87-115">Операційна система Windows 10 виявляє запис точки з'єднання служби (SCP), коли користувач входить на пристрій.</span><span class="sxs-lookup"><span data-stu-id="9cd87-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="9cd87-116">Спочатку пристрій спробує отримати відомості про клієнта з надбудови "клієнт" у реєстрі [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="9cd87-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="9cd87-117">Докладні відомості наведено в статті [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="9cd87-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="9cd87-118">Якщо це не вдасться, пристрій спілкується з локальною службою Active Directory, щоб отримати відомості про клієнта з SCP.</span><span class="sxs-lookup"><span data-stu-id="9cd87-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="9cd87-119">Щоб перевірити, чи передати цей [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="9cd87-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="9cd87-120">Ми рекомендуємо ввімкнути SCP у службі Active Directory та лише за допомогою клієнта SCP для початкової перевірки.</span><span class="sxs-lookup"><span data-stu-id="9cd87-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="9cd87-121">Операційна система Windows 10 намагається спілкуватися з Azure AD в контексті системи, щоб автентифікувати себе від Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9cd87-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="9cd87-122">Ви можете перевірити, чи пристрій може отримати доступ до ресурсів Microsoft у системному обліковому записі за допомогою [сценарію підключення випробувального пристрою](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="9cd87-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="9cd87-123">У Windows 10 створюється Непідписаний сертифікат і зберігається відповідно до об'єкта комп'ютера в локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9cd87-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="9cd87-124">Для цього потрібно мати можливість прямої видимості для контролера домену.</span><span class="sxs-lookup"><span data-stu-id="9cd87-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="9cd87-125">Об'єкт пристрою, який має сертифікат, буде синхронізовано з Azure AD через Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9cd87-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="9cd87-126">Цикл синхронізації – кожні 30 хвилин за замовчуванням, але це залежить від конфігурації підключення Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9cd87-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="9cd87-127">Щоб отримати докладні відомості, зверніться до цього [документа](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="9cd87-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="9cd87-128">На цьому етапі ви зможете побачити тему пристрою в розділі "**очікування**" на пристрої з пристрою лазуровий портал.</span><span class="sxs-lookup"><span data-stu-id="9cd87-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="9cd87-129">Під час входу в обліковий запис до Windows 10 буде завершено реєстрацію.</span><span class="sxs-lookup"><span data-stu-id="9cd87-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9cd87-130">Якщо ви працюєте в мережі VPN, а вихід із системи або вхід припиняється, ви можете ініціювати реєстрацію вручну.</span><span class="sxs-lookup"><span data-stu-id="9cd87-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="9cd87-131">Для цього виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="9cd87-131">To do that:</span></span>
    >
    > <span data-ttu-id="9cd87-132">Видавати `dsregcmd /join` локально на запит адміністратора або віддалено через Pssexec на свій комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="9cd87-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="9cd87-133">Наприклад: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="9cd87-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="9cd87-134">Для поширених проблем із реєстрацією пристроїв Azure Active Directory перегляньте розділ [запитання й відповіді](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="9cd87-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
