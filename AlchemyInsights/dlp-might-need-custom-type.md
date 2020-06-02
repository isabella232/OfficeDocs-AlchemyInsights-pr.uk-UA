---
title: ЗВД може знадобитися користувацький тип
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507535"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="416ea-102">ЗВД може знадобитися користувацький тип</span><span class="sxs-lookup"><span data-stu-id="416ea-102">DLP might need a custom type</span></span>

<span data-ttu-id="416ea-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="416ea-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="416ea-104">**ЗВД може вимагати тип настроюваної інформації**</span><span class="sxs-lookup"><span data-stu-id="416ea-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="416ea-105">За допомогою політики запобігання втрати даних (ЗВД) можна визначити та захистити конфіденційні дані в організації.</span><span class="sxs-lookup"><span data-stu-id="416ea-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="416ea-106">У деяких випадках може знадобитися **створити власний тип конфіденційної інформації** для захисту даних організації.</span><span class="sxs-lookup"><span data-stu-id="416ea-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="416ea-107">Наприклад, ваша організація може потребувати ідентифікації та захисту ідентифікаторів співробітника або інших даних у певному форматі, що стосується вашої організації. Якщо так, зверніться до таких статей, щоб отримати додаткові відомості.</span><span class="sxs-lookup"><span data-stu-id="416ea-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="416ea-108">**Настроювання вбудованого типу конфіденційної інформації**</span><span class="sxs-lookup"><span data-stu-id="416ea-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="416ea-109">Якщо вбудований тип конфіденційної інформації відповідає вашим потребам лише за кілька налаштувань, можна [настроїти вбудований тип конфіденційної інформації](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="416ea-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="416ea-110">Наприклад, можна додати або видалити ключові слова, а також додати або видалити допоміжні докази, наприклад дату або адресу.</span><span class="sxs-lookup"><span data-stu-id="416ea-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="416ea-111">**Створення настроюваного типу даних делікатного характеру**</span><span class="sxs-lookup"><span data-stu-id="416ea-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="416ea-112">Але якщо потрібно, щоб визначити та захистити інший тип конфіденційної інформації в цілому, можна [створити настроюваний тип інформації](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) в інтерфейсі користувача, & відповідність центру безпеки.</span><span class="sxs-lookup"><span data-stu-id="416ea-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="416ea-113">**Створення настроюваного типу конфіденційної інформації в безпеки & центр відповідності PowerShell**</span><span class="sxs-lookup"><span data-stu-id="416ea-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="416ea-114">Нарешті, якщо інтерфейс користувача не надає всі потрібні параметри, можна [створити настроюваний тип інформації в центрі безпеки & відповідності](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="416ea-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="416ea-115">Починаючи з XML-файлу, можна використовувати всі доступні опції.</span><span class="sxs-lookup"><span data-stu-id="416ea-115">By starting with an XML file, you can use every option available.</span></span>
