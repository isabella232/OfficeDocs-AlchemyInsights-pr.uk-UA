---
title: Не вдається активувати Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812593"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="94e02-102">Не вдається активувати Office</span><span class="sxs-lookup"><span data-stu-id="94e02-102">Unable to activate Office</span></span>

- <span data-ttu-id="94e02-103">Перевірте, чи не минув термін дії передплати.</span><span class="sxs-lookup"><span data-stu-id="94e02-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="94e02-104">Переконайтеся, що у вас є передплата, яка підтримує клієнтські ліцензії, як-от Office 365 Business або Office 365 Business преміум, і що [користувачу призначено ліцензію](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="94e02-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="94e02-105">Переконайтеся, що користувач входить в Office за допомогою облікового запису, якому призначено ліцензію.</span><span class="sxs-lookup"><span data-stu-id="94e02-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="94e02-106">Перегляньте [сторінку справності служб Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health), щоб перевірити наявність відомих проблем зі службою.</span><span class="sxs-lookup"><span data-stu-id="94e02-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="94e02-107">Перевірте брандмауер, антивірусну програму та параметри проксі-сервера, щоб переконатися, що вони не блокують доступ програм Microsoft 365 до Інтернету.</span><span class="sxs-lookup"><span data-stu-id="94e02-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="94e02-108">Див. статтю [Діапазони URL- і IP-адрес Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Діапазони URL- і IP-адрес Office 365").</span><span class="sxs-lookup"><span data-stu-id="94e02-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="94e02-109">**Порада.** На комп’ютерах із Windows ми можемо діагностувати та автоматично усунути кілька поширених проблем із входом у систему Office.</span><span class="sxs-lookup"><span data-stu-id="94e02-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="94e02-110">Завантажте та запустіть  **[Помічник із підтримки й відновлення від Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**, щоб скористатися нашим автоматизованим інструментом.</span><span class="sxs-lookup"><span data-stu-id="94e02-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="94e02-111">Виконайте наступні дії з виправлення неполадок:</span><span class="sxs-lookup"><span data-stu-id="94e02-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="94e02-112">Відкрийте програму Office і [вийдіть](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) з будь-якого наявного облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="94e02-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="94e02-113">[Видаліть](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) та [повторно призначте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ліцензію Office, а потім [увійдіть в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9), використовуючи обліковий запис користувача.</span><span class="sxs-lookup"><span data-stu-id="94e02-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="94e02-114">Запустіть [Засіб вирішення проблем активації](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="94e02-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="94e02-115">Скиньте стан активації Office</span><span class="sxs-lookup"><span data-stu-id="94e02-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Скидання стану активації Office")
- [<span data-ttu-id="94e02-116">Виконайте відновлення з мережі для пакета Office</span><span class="sxs-lookup"><span data-stu-id="94e02-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="94e02-117">Додаткові способи виправлення неполадок див. в статтях:</span><span class="sxs-lookup"><span data-stu-id="94e02-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="94e02-118">Помилки про "неліцензований продукт" і помилки активації в Office</span><span class="sxs-lookup"><span data-stu-id="94e02-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="94e02-119">Помилка "На жаль, не вдалося підключитися до облікового запису. Спробуйте ще раз пізніше" під час активації Office</span><span class="sxs-lookup"><span data-stu-id="94e02-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)