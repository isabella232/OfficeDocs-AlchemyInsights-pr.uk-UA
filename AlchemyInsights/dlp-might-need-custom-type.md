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
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932679"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="66b5a-102">ЗВД може знадобитися користувацький тип</span><span class="sxs-lookup"><span data-stu-id="66b5a-102">DLP might need a custom type</span></span>

<span data-ttu-id="66b5a-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="66b5a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="66b5a-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="66b5a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="66b5a-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="66b5a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="66b5a-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="66b5a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="66b5a-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="66b5a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="66b5a-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="66b5a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="66b5a-109">**ЗВД може вимагати тип настроюваної інформації**</span><span class="sxs-lookup"><span data-stu-id="66b5a-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="66b5a-110">За допомогою політики запобігання втрати даних (ЗВД) можна визначити та захистити конфіденційні дані в організації.</span><span class="sxs-lookup"><span data-stu-id="66b5a-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="66b5a-111">У деяких випадках може знадобитися **створити власний тип конфіденційної інформації** для захисту даних організації.</span><span class="sxs-lookup"><span data-stu-id="66b5a-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="66b5a-112">Наприклад, ваша організація може потребувати ідентифікації та захисту ідентифікаторів співробітника або інших даних у певному форматі, що стосується вашої організації. Якщо так, зверніться до таких статей, щоб отримати додаткові відомості.</span><span class="sxs-lookup"><span data-stu-id="66b5a-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="66b5a-113">**Настроювання вбудованого типу конфіденційної інформації**</span><span class="sxs-lookup"><span data-stu-id="66b5a-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="66b5a-114">Якщо вбудований тип конфіденційної інформації відповідає вашим потребам лише за кілька налаштувань, можна [настроїти вбудований тип конфіденційної інформації](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="66b5a-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="66b5a-115">Наприклад, можна додати або видалити ключові слова, а також додати або видалити допоміжні докази, наприклад дату або адресу.</span><span class="sxs-lookup"><span data-stu-id="66b5a-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="66b5a-116">**Створення настроюваного типу даних делікатного характеру**</span><span class="sxs-lookup"><span data-stu-id="66b5a-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="66b5a-117">Але якщо потрібно, щоб визначити та захистити інший тип конфіденційної інформації в цілому, можна [створити настроюваний тип інформації](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) в інтерфейсі користувача, & відповідність центру безпеки.</span><span class="sxs-lookup"><span data-stu-id="66b5a-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="66b5a-118">**Створення настроюваного типу конфіденційної інформації в безпеки & центр відповідності PowerShell**</span><span class="sxs-lookup"><span data-stu-id="66b5a-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="66b5a-119">Нарешті, якщо інтерфейс користувача не надає всі потрібні параметри, можна [створити настроюваний тип інформації в центрі безпеки & відповідності](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="66b5a-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="66b5a-120">Починаючи з XML-файлу, можна використовувати всі доступні опції.</span><span class="sxs-lookup"><span data-stu-id="66b5a-120">By starting with an XML file, you can use every option available.</span></span>
