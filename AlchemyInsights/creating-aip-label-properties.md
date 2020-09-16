---
title: Створення політик підписів AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732196"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a12bf-102">Створення політик підписів AIP</span><span class="sxs-lookup"><span data-stu-id="a12bf-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a12bf-103">Поштові позначки (AIP) можна використовувати з усіма даними, які організація зазвичай створює та зберігає, від найменшого класифікації особистих даних, до найвищої класифікації дуже конфіденційних даних.</span><span class="sxs-lookup"><span data-stu-id="a12bf-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a12bf-104">Політики захисту інформації Azure звертаються до класичного клієнта "Лазурний" (AIP), а не  [клієнта з етикеткою AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="a12bf-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a12bf-105">Можна настроїти кілька елементів політики AIP, зокрема такі параметри, як:</span><span class="sxs-lookup"><span data-stu-id="a12bf-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a12bf-106">Параметр, для якого підпис дасть змогу адміністраторам або класифікувати користувачів і захищати (необов'язково) документи та повідомлення електронної пошти</span><span class="sxs-lookup"><span data-stu-id="a12bf-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a12bf-107">Параметр для застосування класифікації, коли користувачі зберігають документи та надсилають повідомлення електронної пошти</span><span class="sxs-lookup"><span data-stu-id="a12bf-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a12bf-108">Параметр, щоб автоматично позначити повідомлення електронної пошти на основі вкладень.</span><span class="sxs-lookup"><span data-stu-id="a12bf-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a12bf-109">Параметр, який дає змогу визначити, чи відображається панель захисту інформації в програмах Office</span><span class="sxs-lookup"><span data-stu-id="a12bf-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a12bf-110">Щоб отримати додаткові можливості та відомості про політики захисту даних Azure, див.: [Огляд політики захисту інформації в Лазур](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="a12bf-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a12bf-111">Для інших корисних ресурсів, які стосуються політики AIP, див.:</span><span class="sxs-lookup"><span data-stu-id="a12bf-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a12bf-112">Навчальний посібник: настроювання параметрів політики захисту даних Azure і створення нової етикетки</span><span class="sxs-lookup"><span data-stu-id="a12bf-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a12bf-113">Налаштування політики захисту інформації в Лазур</span><span class="sxs-lookup"><span data-stu-id="a12bf-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a12bf-114">Створення та настроювання міток конфіденційності та їх політики</span><span class="sxs-lookup"><span data-stu-id="a12bf-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a12bf-115">Посібники для поширених сценаріїв, які використовують захист інформації Azure</span><span class="sxs-lookup"><span data-stu-id="a12bf-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a12bf-116">Огляд документації з захисту інформації про Azure</span><span class="sxs-lookup"><span data-stu-id="a12bf-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a12bf-117">Вимоги для захисту інформації за Azure</span><span class="sxs-lookup"><span data-stu-id="a12bf-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a12bf-118">Короткий посібник із захисту інформації для Azure</span><span class="sxs-lookup"><span data-stu-id="a12bf-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a12bf-119">Завантажити клієнт захисту даних Azure</span><span class="sxs-lookup"><span data-stu-id="a12bf-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)