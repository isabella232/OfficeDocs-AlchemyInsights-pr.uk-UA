---
title: Усунення помилок, що вказували на "неліцензований продукт"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786870"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="e4842-102">Пропозиції щодо виправлення помилок "Неліцензований продукт"</span><span class="sxs-lookup"><span data-stu-id="e4842-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="e4842-103">Щоб усунути помилки про "неліцензований продукт", спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="e4842-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="e4842-104">Перевірте, чи не завершиться термін дії вашої передплати.</span><span class="sxs-lookup"><span data-stu-id="e4842-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="e4842-105">Переконайтеся, що у вас є передплата, яка дає змогу клієнтським ліцензіям, наприклад програмам Microsoft 365 для бізнесу або "Business преміум", і переконайтеся, що [користувачу призначено ліцензію.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="e4842-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="e4842-106">Переконайтеся, що користувач входив в Office за допомогою того самого облікового запису, у який призначено ліцензію.</span><span class="sxs-lookup"><span data-stu-id="e4842-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e4842-107">На сторінці [Справність служби](https://docs.microsoft.com/office365/enterprise/view-service-health) перевірте, чи немає відомих проблем зі службою.</span><span class="sxs-lookup"><span data-stu-id="e4842-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e4842-108">Перевірте параметри брандмауера, антивірусного програмного забезпечення та проксі-сервера, щоб переконатися, що вони не блокують доступ програм Microsoft 365 до Інтернету.</span><span class="sxs-lookup"><span data-stu-id="e4842-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="e4842-109">Див. [номери URL-адрес і діапазони IP-адрес.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="e4842-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="e4842-110">Крім того, можна спробувати виконати наведені нижче дії з виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="e4842-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="e4842-111">Відкрийте програму Office і вийдіть [із наявних](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) облікових записів користувачів.</span><span class="sxs-lookup"><span data-stu-id="e4842-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e4842-112">[Видаліть](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) і [повторно призначте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ліцензію Office, а потім увійдіть в [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) за допомогою відповідного облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="e4842-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e4842-113">Запустіть засіб [усунення неполадок активації](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="e4842-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="e4842-114">[Скиньте стан активації Office.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="e4842-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="e4842-115">[Виконайте відновлення з мережі для пакета Office.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="e4842-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="e4842-116">Додаткові способи виправлення неполадок див. в статтях:</span><span class="sxs-lookup"><span data-stu-id="e4842-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="e4842-117">Помилки про "неліцензований продукт" і помилки активації в Office</span><span class="sxs-lookup"><span data-stu-id="e4842-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="e4842-118">Помилка "На жаль, не вдалося підключитися до облікового запису. Спробуйте ще раз пізніше" під час активації Office</span><span class="sxs-lookup"><span data-stu-id="e4842-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)