---
title: У мене заблоковано умовний доступ до пристрою, до якого приєднується домен
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038107"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="d888f-102">У мене заблоковано умовний доступ до пристрою, до якого приєднується домен</span><span class="sxs-lookup"><span data-stu-id="d888f-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="d888f-103">**Високорекомендовані інструменти**</span><span class="sxs-lookup"><span data-stu-id="d888f-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="d888f-104">Засіб [вирішення проблем із реєстрацією пристроїв](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – засіб, який допомагає у виправленні неполадок із найпоширенішим питанням реєстрації пристроїв.</span><span class="sxs-lookup"><span data-stu-id="d888f-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="d888f-105">[Сценарій підключення пристрою для тестування](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : сценарій, який допомагає забезпечити, щоб пристрій міг отримати доступ до кінцевих точок реєстрації пристрою в системному обліковому записі.</span><span class="sxs-lookup"><span data-stu-id="d888f-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="d888f-106">[Скрипт очищення пристрою в Лазур](https://github.com/mzmaili/AzureADDeviceCleanup) – скрипт, який дає змогу шукати та керувати застарілою пристроями в навколишньому середовищі.</span><span class="sxs-lookup"><span data-stu-id="d888f-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="d888f-107">Нижче наведено кілька типових причин, через які умовний доступ може не працювати з пристроєм, який приєднався до домену (гібридне блакитне AD).</span><span class="sxs-lookup"><span data-stu-id="d888f-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="d888f-108">**На пристрої немає лазуроної реклами** – потрібно переконатися, що на пристрої є маркер первинного оновлення «AZURE AD» (PRT).</span><span class="sxs-lookup"><span data-stu-id="d888f-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="d888f-109">Щоб отримати докладніші відомості про PRT, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="d888f-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="d888f-110">Щоб перевірити, чи є у вас блакитний AD PRT, ви можете запустити `dsregcmd/status` команду на пристрої та перевірити, чи "AzureAdPrt" дорівнює "так".</span><span class="sxs-lookup"><span data-stu-id="d888f-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="d888f-111">Якщо "AzureAdPrt" є "ні", перевірте таке:</span><span class="sxs-lookup"><span data-stu-id="d888f-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="d888f-112">**Незалежно від того, чи є у вас федеративне середовище з AD FS, і вона недоступна в домашніх мережах користувачів**: у цьому випадку переконайтеся, що кінцеві точки usernamemed доступні в мережі екстранет.</span><span class="sxs-lookup"><span data-stu-id="d888f-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="d888f-113">Якщо ваше AD FS знаходиться позаду віртуальної приватної мережі, переконайтеся, що користувачі підключаються до мережі VPN і повторно Увійдіть на пристрій.</span><span class="sxs-lookup"><span data-stu-id="d888f-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="d888f-114">Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="d888f-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="d888f-115">**Незалежно від того, що TPM пристрою несправний, і таким чином не можна автентифікувати пристрій**: установіть прапорець "TPM. msc", щоб дізнатися, чи стан модуля TPM "Готово".</span><span class="sxs-lookup"><span data-stu-id="d888f-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="d888f-116">Якщо це не так, запустіть `dsregcmd/leave` і дайте пристрою повторно приєднатися до Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d888f-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="d888f-117">Потім повторіть спробу.</span><span class="sxs-lookup"><span data-stu-id="d888f-117">Then, try again.</span></span> <span data-ttu-id="d888f-118">Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="d888f-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="d888f-119">**Ви використовуєте постачальника посвідчень 3rd Party, який не підтримує протокол WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="d888f-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="d888f-120">Як описано в наших документах, у цьому випадку не можна працювати з гібридним пристроями, підключеному до AD-пристроїв.</span><span class="sxs-lookup"><span data-stu-id="d888f-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="d888f-121">Ви можете працювати з постачальником посвідчень для підтримки.</span><span class="sxs-lookup"><span data-stu-id="d888f-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="d888f-122">**Користувачі, які використовують браузер Chrome без облікових записів Windows 10** або розширення Office, не можуть **автоматично використовувати ГВП на пристроях aad, підключених до мережі або гібридних-aad**. це призводить до провалу будь-яких політик умовного доступу на основі пристрою, у якому відображається повідомлення про помилку "незареєстрований пристрій".</span><span class="sxs-lookup"><span data-stu-id="d888f-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="d888f-123">Щоб правильно використовувати браузер Chrome, потрібно інсталювати "облікові записи Windows 10" або "розширення Office до браузера Chrome" за допомогою SCCM або Inune.</span><span class="sxs-lookup"><span data-stu-id="d888f-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="d888f-124">Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="d888f-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="d888f-125">Якщо ви не можете натиснути розширення віддалено, повідомте користувачів, щоб вручну інсталювати один із наведених вище розширень, щоб отримати доступ до програм за допомогою умовного доступу на основі пристрою.</span><span class="sxs-lookup"><span data-stu-id="d888f-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="d888f-126">Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="d888f-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="d888f-127">**Пристрій був належним чином видалений, але його було видалено або вимкнуто через синхронізацію в AZURE AD Connect або на порталі Azure**: якщо це станеться, об'єкт пристрою більше не розпізнається як повністю підключений пристрій, хоча стан "AzureAdJoined" і "PRT" відображається як дійсний на пристрої.</span><span class="sxs-lookup"><span data-stu-id="d888f-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="d888f-128">Щоб вирішити цю проблему, запустіть `dsregcmd/leave` їх на уражених пристроях і дайте їм змогу повторно приєднатися до "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="d888f-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="d888f-129">Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="d888f-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="d888f-130">Якщо ваші пристрої знаходяться в ОС Windows 10, 1809 Update, з проксі-сервером VPN/Cloud і в разі виникнення проблем із "AzureAdPrt" або будь-якою програмою з помилкою єдиного входу (програма Outlook не підключається до поштової скриньки, навіть якщо у вас є PRT), переконайтеся, що ви маєте цей патч [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) або квітня накопичувальне оновлення [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , щоб запобігти появі збоїв ГВП на цих машинах</span><span class="sxs-lookup"><span data-stu-id="d888f-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















