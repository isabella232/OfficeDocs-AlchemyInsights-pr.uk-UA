---
title: Можливо, знадобиться настроюваний тип DLP.
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712205"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="4eccf-102">Можливо, знадобиться настроюваний тип DLP.</span><span class="sxs-lookup"><span data-stu-id="4eccf-102">DLP might need a custom type</span></span>

<span data-ttu-id="4eccf-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4eccf-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4eccf-104">**Для DLP може знадобитися настроюваний тип інформації**</span><span class="sxs-lookup"><span data-stu-id="4eccf-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="4eccf-105">За допомогою політики запобігання втраті даних (DLP) можна ідентифікувати та захистити конфіденційні дані в організації.</span><span class="sxs-lookup"><span data-stu-id="4eccf-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="4eccf-106">У деяких сценаріях, можливо, знадобиться створити власний **настроюваний** тип конфіденційної інформації, щоб захистити дані вашої організації.</span><span class="sxs-lookup"><span data-stu-id="4eccf-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="4eccf-107">Наприклад, у вашій організації може знадобитися визначити та захистити ідентифікатори працівників або інші дані в певному форматі, які стосуються організаційної організації. Якщо так, перегляньте наведені нижче статті, щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="4eccf-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="4eccf-108">**Настроювання вбудованого чутливе типу відомостей**</span><span class="sxs-lookup"><span data-stu-id="4eccf-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="4eccf-109">Якщо вбудований тип інформації буде відповідно до ваших потреб за допомогою кількох настройок, можна [настроїти вбудований тип конфіденційної інформації](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="4eccf-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="4eccf-110">Наприклад, можна додати або видалити ключові слова або додати або видалити допоміжні свідчення, як-от дату або адресу.</span><span class="sxs-lookup"><span data-stu-id="4eccf-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="4eccf-111">**Створення спеціального чутливе типу відомостей**</span><span class="sxs-lookup"><span data-stu-id="4eccf-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="4eccf-112">Але якщо потрібно ідентифікувати та захистити інший тип конфіденційної інформації, можна [створити настроюваний чутливий тип інформації](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) в інтерфейсі відповідності центру безпеки &.</span><span class="sxs-lookup"><span data-stu-id="4eccf-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="4eccf-113">**Створення настроюваної конфіденційної інформації в центрі безпеки & відповідності центру PowerShell**</span><span class="sxs-lookup"><span data-stu-id="4eccf-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="4eccf-114">Нарешті, якщо для інтерфейсу користувача не передбачено всі потрібні параметри, можна [створити настроюваний чутливий тип інформації в центрі безпеки & відповідність PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="4eccf-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="4eccf-115">Починаючи з XML-файлу, можна використовувати всі доступні параметри.</span><span class="sxs-lookup"><span data-stu-id="4eccf-115">By starting with an XML file, you can use every option available.</span></span>
