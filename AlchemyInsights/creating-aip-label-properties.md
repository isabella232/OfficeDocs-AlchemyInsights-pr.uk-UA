---
title: Створення політики маркування AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569516"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="73b19-102">Створення політики маркування AIP</span><span class="sxs-lookup"><span data-stu-id="73b19-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="73b19-103">Підписи захисту інформації (AIP) можна використовувати з повним діапазоном даних, які організація зазвичай створює та зберігає від найнижчої класифікації особистих даних, до найвищої класифікації високо конфіденційних даних.</span><span class="sxs-lookup"><span data-stu-id="73b19-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="73b19-104">Azure відомості про захист політики застосовуються до Azure відомості про захист (AIP) класичний клієнт, а не [AIP уніфікований маркування клієнта](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="73b19-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="73b19-105">Ви можете налаштувати кілька елементів у політиці AIP, включаючи такі параметри:</span><span class="sxs-lookup"><span data-stu-id="73b19-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="73b19-106">Параметр, для якого підпис дозволить адміністраторам або класифікувати та захист користувачів (необов'язково) документи та електронні листи</span><span class="sxs-lookup"><span data-stu-id="73b19-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="73b19-107">Можливість застосування класифікації під час збереження документів і надсилання повідомлень електронної пошти</span><span class="sxs-lookup"><span data-stu-id="73b19-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="73b19-108">Можливість автоматично позначити повідомлення електронної пошти на основі його вкладень.</span><span class="sxs-lookup"><span data-stu-id="73b19-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="73b19-109">Можливість контролювати, чи відображається панель захисту інформації в застосунках Office</span><span class="sxs-lookup"><span data-stu-id="73b19-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="73b19-110">Додаткові параметри та відомості про політику захисту інформації Azure див.: [Огляд політики захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="73b19-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="73b19-111">Для інших корисних ресурсів, що стосуються політики AIP, див.:</span><span class="sxs-lookup"><span data-stu-id="73b19-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="73b19-112">Посібник: настроювання параметрів політики захисту інформації в Azure та створення нової етикетки</span><span class="sxs-lookup"><span data-stu-id="73b19-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="73b19-113">Налаштування політики захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="73b19-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="73b19-114">Створення та настроювання міток чутливості та їх політик</span><span class="sxs-lookup"><span data-stu-id="73b19-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="73b19-115">Інструкції для поширених сценаріїв, які використовують Azure захисту інформації</span><span class="sxs-lookup"><span data-stu-id="73b19-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="73b19-116">Огляд документації з захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="73b19-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="73b19-117">Вимоги для захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="73b19-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="73b19-118">Короткий посібник з захисту інформації для Azure</span><span class="sxs-lookup"><span data-stu-id="73b19-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="73b19-119">Завантажити клієнт для захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="73b19-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)