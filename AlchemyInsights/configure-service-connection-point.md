---
title: Настроювання точки з'єднання служби (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037293"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="1d3f1-102">Настроювання точки з'єднання служби (SCP)</span><span class="sxs-lookup"><span data-stu-id="1d3f1-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="1d3f1-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c 001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="1d3f1-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="1d3f1-104">**Причина**: не вдається прочитати об'єкт scp і отримати відомості про клієнта AZURE AD</span><span class="sxs-lookup"><span data-stu-id="1d3f1-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="1d3f1-105">**Роздільна здатність**: посилання на розділ [Настроювання точки з'єднання служби](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="1d3f1-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="1d3f1-106">**План дій**</span><span class="sxs-lookup"><span data-stu-id="1d3f1-106">**Action plan**</span></span>

- <span data-ttu-id="1d3f1-107">Перевірте, чи отримали пристрій GPO для контрольованого перевірки.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="1d3f1-108">Переконайтеся, що об'єкт групової політики створив розділи реєстру.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="1d3f1-109">Переконайтеся, що у вас є 2 клавіші, створені за допомогою ІДЕНТИФІКАТОРА каталогів і домену onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="1d3f1-110">**Настроювання клієнтського реєстру для SCP**</span><span class="sxs-lookup"><span data-stu-id="1d3f1-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="1d3f1-111">Використовуйте наведений нижче приклад, щоб створити об'єкт групової політики (GPO), щоб розгорнути параметр реєстру, який настроює запис SCP в реєстрі пристроїв.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="1d3f1-112">Відкрийте консоль керування груповою політикою та створіть новий об'єкт групової політики в домені.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="1d3f1-113">Надання новоствореного імені групової політики (наприклад, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="1d3f1-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="1d3f1-114">Відредагуйте об'єкт групової політики та знайдіть такий шлях: налаштування **конфігурації комп'ютера > > настройки Windows > реєстрі**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="1d3f1-115">Клацніть правою кнопкою миші **реєстр** та виберіть **елемент новий > реєстру**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="1d3f1-116">На вкладці **загальні** настройте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="1d3f1-117">**Дія**: оновлення</span><span class="sxs-lookup"><span data-stu-id="1d3f1-117">**Action**: Update</span></span>
    
- <span data-ttu-id="1d3f1-118">**Вулик**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="1d3f1-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="1d3f1-119">**Шлях до ключа**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="1d3f1-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="1d3f1-120">**Ім'я значення**: tenantid</span><span class="sxs-lookup"><span data-stu-id="1d3f1-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="1d3f1-121">**Тип значення**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="1d3f1-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="1d3f1-122">**Значення даних**: GUID або ідентифікатор каталогу в екземплярі AZURE AD (це значення можна знайти на **порталі azure Portal > azure Active directory > властивості > ідентифікатор каталогу**)</span><span class="sxs-lookup"><span data-stu-id="1d3f1-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="1d3f1-123">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="1d3f1-124">Клацніть правою кнопкою миші **реєстр** та виберіть **елемент новий > реєстру**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="1d3f1-125">На вкладці **загальні** настройте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="1d3f1-126">**Дія**: оновлення</span><span class="sxs-lookup"><span data-stu-id="1d3f1-126">**Action**: Update</span></span>
    
- <span data-ttu-id="1d3f1-127">**Вулик**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="1d3f1-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="1d3f1-128">**Шлях до ключа**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="1d3f1-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="1d3f1-129">**Ім'я _ значення**: ім'я для tenantname</span><span class="sxs-lookup"><span data-stu-id="1d3f1-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="1d3f1-130">**Тип значення**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="1d3f1-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="1d3f1-131">**Значення даних**: перевірену назву домену, якщо використовується інтегроване середовище, наприклад AD FS.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="1d3f1-132">Перевірену назву домену або ім'я домену onmicrosoft.com (наприклад, contoso. onmicrosoft). com, якщо використовується кероване середовище</span><span class="sxs-lookup"><span data-stu-id="1d3f1-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="1d3f1-133">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-133">Click **OK**.</span></span>

7. <span data-ttu-id="1d3f1-134">Закрийте редактор для щойно створеного об'єкта групової політики.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="1d3f1-135">Зв'яжіть щойно створений об'єкт групової політики, у якому містяться підключені до домену комп'ютери, які належать до списку контрольованих свиті.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="1d3f1-136">Докладні відомості наведено в статті [контрольована перевірка гібридного AD JOIN-Azure Документи Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) і  [Виправлення неполадок із гібридним Лазурний Active Directory | Документи Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="1d3f1-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









