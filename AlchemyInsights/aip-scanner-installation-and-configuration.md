---
title: 'AIP scanner: installation and configuration'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821684"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="48e8f-102">AIP scanner: installation and configuration</span><span class="sxs-lookup"><span data-stu-id="48e8f-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="48e8f-103">**Щоб інсталювати сканер AIP, дотримуйтеся рекомендованих рекомендацій:**</span><span class="sxs-lookup"><span data-stu-id="48e8f-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="48e8f-104">Якщо ви виконуєте чисту інсталяцію, але не виконуєте чисту інсталяцію, переконайтеся, що ви дотримувалися рекомендацій з оновлення сканера [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) і клієнта уніфікованого підписування, див. номери оновлення засобу перевірки захисту даних [Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="48e8f-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="48e8f-105">Переконайтеся, що ви відповідаєте всім вимогам до [брандмауерів і інфраструктури мережі.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="48e8f-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="48e8f-106">Переконайтеся, [що політики настроєно на](https://docs.microsoft.com/azure/information-protection/configure-policy) автоматичне підписування, або призначте політикі стандартну мітку.</span><span class="sxs-lookup"><span data-stu-id="48e8f-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="48e8f-107">Переконайтеся, що для відповідного типу файлу настроєно етикетку або захист, як описано в розділі Типи файлів, які підтримує клієнт [Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="48e8f-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="48e8f-108">Крім того, якщо потрібно змінити стандартну поведінку, дотримуйтеся наведених нижче порад: Змінення рівня захисту файлів [за замовчуванням.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="48e8f-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="48e8f-109">Переконайтеся, що обліковий запис користувача, настроєний для запуску служби сканера, має дозволи на доступ до всіх налаштованих сховищ.</span><span class="sxs-lookup"><span data-stu-id="48e8f-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="48e8f-110">Якщо проблеми не зникнуть, експортуйте журнали сканера та додайте їх до запиту на підтримку.</span><span class="sxs-lookup"><span data-stu-id="48e8f-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="48e8f-111">**Експорт журналів засобу перевірки даних Azure**</span><span class="sxs-lookup"><span data-stu-id="48e8f-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="48e8f-112">Перейдіть до %localappdata%\Microsoft\MSIP у контексті користувача, який виконує службу сканера.</span><span class="sxs-lookup"><span data-stu-id="48e8f-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="48e8f-113">Запакувати весь вміст папки MSIP.</span><span class="sxs-lookup"><span data-stu-id="48e8f-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="48e8f-114">Збережіть журнали у вибраному розташуванні та вкладіть їх у свій запит на обслуговування.</span><span class="sxs-lookup"><span data-stu-id="48e8f-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="48e8f-115">Ви також можете використовувати [Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="48e8f-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="48e8f-116">**Докладні відомості див. в такому:**</span><span class="sxs-lookup"><span data-stu-id="48e8f-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="48e8f-117">Розгортання сканера Azure Information Protection для автоматичного класифікації та захисту файлів</span><span class="sxs-lookup"><span data-stu-id="48e8f-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="48e8f-118">Визначення та використання параметра Token для Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="48e8f-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="48e8f-119">Запуск циклу виявлення та перегляд звітів для сканера</span><span class="sxs-lookup"><span data-stu-id="48e8f-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="48e8f-120">Перегляд документації для захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="48e8f-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="48e8f-121">Вимоги до захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="48e8f-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="48e8f-122">Завантаження клієнта Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="48e8f-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
