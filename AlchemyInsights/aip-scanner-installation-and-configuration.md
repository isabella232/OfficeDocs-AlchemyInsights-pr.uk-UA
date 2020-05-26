---
title: 'AIP сканер: установка і конфігурація'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358570"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="01b76-102">AIP сканер: установка і конфігурація</span><span class="sxs-lookup"><span data-stu-id="01b76-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="01b76-103">**Щоб встановити сканер AIP, дотримуйтеся рекомендованих рекомендацій**:</span><span class="sxs-lookup"><span data-stu-id="01b76-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="01b76-104">Якщо ви оновлюєте і не виконуєте чисту інсталяцію, переконайтеся, що ви виконали вказівки з [оновлення сканера захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) і для уніфікованого позначення клієнта, перегляньте [оновлення сканера захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="01b76-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="01b76-105">Переконайтеся, що ви дотримуєтесь всіх [параметрів брандмауера та настройок мережної інфраструктури](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="01b76-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="01b76-106">Переконайтеся, що для [політики встановлено](https://docs.microsoft.com/azure/information-protection/configure-policy) автоматичне маркування або підпис за промовчанням у політиці.</span><span class="sxs-lookup"><span data-stu-id="01b76-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="01b76-107">Переконайтеся, що відповідний тип файлу настроєно для міток/захисту, як описано в [типах файлів, які підтримуються клієнтом захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="01b76-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="01b76-108">Крім того, якщо потрібно змінити поведінку за промовчанням, дотримуйтеся наведених нижче вказівок. [змінення рівня захисту файлів за промовчанням](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="01b76-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="01b76-109">Переконайтеся, що обліковий запис користувача, настроєний для запуску служби сканера, має дозволи на доступ до всіх настроєних сховищ.</span><span class="sxs-lookup"><span data-stu-id="01b76-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="01b76-110">Якщо виникають проблеми, будь ласка, експортуйте журнали сканера та додайте їх до квитка підтримки.</span><span class="sxs-lookup"><span data-stu-id="01b76-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="01b76-111">**Експортування журналів сканера захисту інформації Azure**</span><span class="sxs-lookup"><span data-stu-id="01b76-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="01b76-112">Перейдіть до%Localappdate%\miceptemclinn, під контекстом користувача, який працює служба сканера.</span><span class="sxs-lookup"><span data-stu-id="01b76-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="01b76-113">ZIP весь вміст у папці MSIP.</span><span class="sxs-lookup"><span data-stu-id="01b76-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="01b76-114">Збережіть журнали на вибір місцеположення та Прикріпіть їх до вашого запиту на обслуговування.</span><span class="sxs-lookup"><span data-stu-id="01b76-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="01b76-115">Ви також можете використовувати [експорт-Aiplмоги-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="01b76-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="01b76-116">**За додатковою інформацією див**.:</span><span class="sxs-lookup"><span data-stu-id="01b76-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="01b76-117">Розгортання в Azure захисту інформації сканер для автоматичної класифікації та захисту файлів</span><span class="sxs-lookup"><span data-stu-id="01b76-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="01b76-118">Укажіть та використайте параметр маркерів для параметра Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="01b76-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="01b76-119">Запуск циклу виявлення та перегляд звітів для сканера</span><span class="sxs-lookup"><span data-stu-id="01b76-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="01b76-120">Огляд документації з захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="01b76-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="01b76-121">Вимоги для захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="01b76-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="01b76-122">Завантажити клієнт для захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="01b76-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
