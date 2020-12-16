---
title: Перенесення служб – переміщення всіх служб RDFE до іншої передплатою
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692425"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="f7afa-102">Перенесення служб – переміщення всіх служб RDFE до іншої передплатою</span><span class="sxs-lookup"><span data-stu-id="f7afa-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="f7afa-103">**Переміщення ресурсів**</span><span class="sxs-lookup"><span data-stu-id="f7afa-103">**Move resources**</span></span>

<span data-ttu-id="f7afa-104">Блакитні ресурси можна переміщати в іншу абонентську або групу ресурсів в межах однієї передплатою, використовуючи Azure Portal, Azure PowerShell, Azure CLI або API REST для переміщення ресурсів.</span><span class="sxs-lookup"><span data-stu-id="f7afa-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="f7afa-105">Перш ніж переходити до ресурсів, див.:</span><span class="sxs-lookup"><span data-stu-id="f7afa-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="f7afa-106">Контрольний список перед переміщенням ресурсів</span><span class="sxs-lookup"><span data-stu-id="f7afa-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="f7afa-107">Служби, які можна переміщати</span><span class="sxs-lookup"><span data-stu-id="f7afa-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f7afa-108">Перевірка переміщення</span><span class="sxs-lookup"><span data-stu-id="f7afa-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="f7afa-109">Переміщення рекомендацій для служб</span><span class="sxs-lookup"><span data-stu-id="f7afa-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="f7afa-110">Щоб перенести доступні ресурси до іншої групи ресурсів або передплатою, можна скористатися:</span><span class="sxs-lookup"><span data-stu-id="f7afa-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="f7afa-111">Портал «Лазурний»</span><span class="sxs-lookup"><span data-stu-id="f7afa-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="f7afa-112">Блакитний PowerShell</span><span class="sxs-lookup"><span data-stu-id="f7afa-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="f7afa-113">Блакитний CLI</span><span class="sxs-lookup"><span data-stu-id="f7afa-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="f7afa-114">API REST</span><span class="sxs-lookup"><span data-stu-id="f7afa-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="f7afa-115">Навчальний посібник: [переміщення блакитного ресурсу до іншої групи ресурсів або передплатою](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="f7afa-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="f7afa-116">**Виправлення неполадок із диспетчером ресурсів Azure**</span><span class="sxs-lookup"><span data-stu-id="f7afa-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="f7afa-117">Зверніться до статей нижче, щоб дізнатися про деякі поширені помилки в Лазурне розгортання та отримувати інформацію, щоб їх вирішити.</span><span class="sxs-lookup"><span data-stu-id="f7afa-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="f7afa-118">Якщо ви не можете знайти код помилки для вашої помилки розгортання, перегляньте статтю [знайти код помилки](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="f7afa-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="f7afa-119">Виправлення помилок розгортання</span><span class="sxs-lookup"><span data-stu-id="f7afa-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="f7afa-120">Виправлення неполадок із переміщенням лазурових ресурсів до нової групи ресурсів або передплатою</span><span class="sxs-lookup"><span data-stu-id="f7afa-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="f7afa-121">Зверніть увагу, що якщо ви хочете оновити свою безкоштовну передплатну розсилку, наприклад перехід від безкоштовного до оплати, як-от-го, вам потрібно буде перетворити свою абонентську плату.</span><span class="sxs-lookup"><span data-stu-id="f7afa-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="f7afa-122">Щоб оновити безкоштовну ознайомлювальну версію, ознайомтеся з [оновленням безкоштовного ознайомлювального або Microsoft Уявіть, що ви хочете сплатити за передплату](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="f7afa-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="f7afa-123">Щоб змінити обліковий запис "сплатити за вас", Дізнайтеся, [як перейти до іншої пропозиції](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="f7afa-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="f7afa-124">**Щоб додати або пов'язати "Лазурний" для клієнта Azure Active Directory, зробіть ось що:**</span><span class="sxs-lookup"><span data-stu-id="f7afa-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="f7afa-125">Увійдіть у службу та виберіть передплату, яку потрібно використовувати на [сторінці "передплати" на порталі Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="f7afa-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="f7afa-126">Виберіть **змінити каталог**.</span><span class="sxs-lookup"><span data-stu-id="f7afa-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="f7afa-127">Перегляньте всі попередження, які відображатимуться, а потім натисніть кнопку **змінити**.</span><span class="sxs-lookup"><span data-stu-id="f7afa-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="f7afa-128">Каталог буде змінений для передплатою, і ви отримаєте повідомлення про успішне.</span><span class="sxs-lookup"><span data-stu-id="f7afa-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="f7afa-129">Скористайтеся перемикачем *каталогів* , щоб перейти до нового каталогу.</span><span class="sxs-lookup"><span data-stu-id="f7afa-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="f7afa-130">Це може тривати до 10 хвилин, щоб усі відображалися належним чином.</span><span class="sxs-lookup"><span data-stu-id="f7afa-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="f7afa-131">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="f7afa-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="f7afa-132">Передача права власності на Лазурне</span><span class="sxs-lookup"><span data-stu-id="f7afa-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="f7afa-133">Переміщення ресурсів до нової групи ресурсів або передплатою</span><span class="sxs-lookup"><span data-stu-id="f7afa-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="f7afa-134">Керування ресурсами за допомогою порталу "Лазурний"</span><span class="sxs-lookup"><span data-stu-id="f7afa-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
