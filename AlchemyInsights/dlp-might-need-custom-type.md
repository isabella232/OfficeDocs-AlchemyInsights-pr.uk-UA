---
title: ЗВД може знадобитися користувацький тип
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977291"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="03390-102">ЗВД може знадобитися користувацький тип</span><span class="sxs-lookup"><span data-stu-id="03390-102">DLP might need a custom type</span></span>

<span data-ttu-id="03390-103">**Важливо**: у ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються доступними – будь ласка, відвідайте [тимчасові функції SharePoint Online](https://aka.ms/ODSPAdjustments) для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="03390-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="03390-104">**ЗВД може вимагати тип настроюваної інформації**</span><span class="sxs-lookup"><span data-stu-id="03390-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="03390-105">За допомогою політики запобігання втрати даних (ЗВД) можна визначити та захистити конфіденційні дані в організації.</span><span class="sxs-lookup"><span data-stu-id="03390-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="03390-106">У деяких випадках може знадобитися **створити власний тип конфіденційної інформації** для захисту даних організації.</span><span class="sxs-lookup"><span data-stu-id="03390-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="03390-107">Наприклад, ваша організація може потребувати ідентифікації та захисту ідентифікаторів співробітника або інших даних у певному форматі, що стосується вашої організації. Якщо так, зверніться до таких статей, щоб отримати додаткові відомості.</span><span class="sxs-lookup"><span data-stu-id="03390-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="03390-108">**Настроювання вбудованого типу конфіденційної інформації**</span><span class="sxs-lookup"><span data-stu-id="03390-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="03390-109">Якщо вбудований тип конфіденційної інформації відповідає вашим потребам лише за кілька налаштувань, можна [настроїти вбудований тип конфіденційної інформації](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="03390-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="03390-110">Наприклад, можна додати або видалити ключові слова, а також додати або видалити допоміжні докази, наприклад дату або адресу.</span><span class="sxs-lookup"><span data-stu-id="03390-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="03390-111">**Створення настроюваного типу даних делікатного характеру**</span><span class="sxs-lookup"><span data-stu-id="03390-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="03390-112">Але якщо потрібно, щоб визначити та захистити інший тип конфіденційної інформації в цілому, можна [створити настроюваний тип інформації](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) в інтерфейсі користувача, & відповідність центру безпеки.</span><span class="sxs-lookup"><span data-stu-id="03390-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="03390-113">**Створення настроюваного типу конфіденційної інформації в безпеки & центр відповідності PowerShell**</span><span class="sxs-lookup"><span data-stu-id="03390-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="03390-114">Нарешті, якщо інтерфейс користувача не надає всі потрібні параметри, можна [створити настроюваний тип інформації в центрі безпеки & відповідності](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="03390-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="03390-115">Починаючи з XML-файлу, можна використовувати всі доступні опції.</span><span class="sxs-lookup"><span data-stu-id="03390-115">By starting with an XML file, you can use every option available.</span></span>
