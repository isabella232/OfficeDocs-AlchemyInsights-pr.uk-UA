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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798701"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="4373c-102">Не вдається активувати Office</span><span class="sxs-lookup"><span data-stu-id="4373c-102">Unable to activate Office</span></span>

<span data-ttu-id="4373c-103">**Примітка.** Якщо використовується попередня версія Windows (наприклад, Windows 7), переконайтеся, що протокол TLS 1.2 ввімкнуто за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="4373c-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="4373c-104">Докладні відомості див. в статтях Оновлення для ввімкнення [протоколів TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)як безпечних протоколів за замовчуванням у WindowsHTTP у Windows.</span><span class="sxs-lookup"><span data-stu-id="4373c-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="4373c-105">Перевірте, чи не минув термін дії передплати.</span><span class="sxs-lookup"><span data-stu-id="4373c-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="4373c-106">Переконайтеся, що у вас є передплата, яка підтримує клієнтські ліцензії, як-от Office 365 Business або Office 365 Business преміум, і що [користувачу призначено ліцензію](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="4373c-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="4373c-107">Переконайтеся, що користувач входить в Office за допомогою облікового запису, якому призначено ліцензію.</span><span class="sxs-lookup"><span data-stu-id="4373c-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="4373c-108">Перегляньте [сторінку справності служб Office 365](/office365/enterprise/view-service-health), щоб перевірити наявність відомих проблем зі службою.</span><span class="sxs-lookup"><span data-stu-id="4373c-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="4373c-109">Перевірте брандмауер, антивірусну програму та параметри проксі-сервера, щоб переконатися, що вони не блокують доступ програм Microsoft 365 до Інтернету.</span><span class="sxs-lookup"><span data-stu-id="4373c-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="4373c-110">Див. статтю [Діапазони URL- і IP-адрес Office 365](/office365/enterprise/urls-and-ip-address-ranges "Діапазони URL- і IP-адрес Office 365").</span><span class="sxs-lookup"><span data-stu-id="4373c-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="4373c-111">**Порада.** На комп’ютерах із Windows ми можемо діагностувати та автоматично усунути кілька поширених проблем із входом у систему Office.</span><span class="sxs-lookup"><span data-stu-id="4373c-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="4373c-112">Завантажте та запустіть  **[Помічник із підтримки й відновлення від Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**, щоб скористатися нашим автоматизованим інструментом.</span><span class="sxs-lookup"><span data-stu-id="4373c-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="4373c-113">Виконайте наступні дії з виправлення неполадок:</span><span class="sxs-lookup"><span data-stu-id="4373c-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="4373c-114">Відкрийте програму Office і [вийдіть](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) з будь-якого наявного облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="4373c-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="4373c-115">[Видаліть](/microsoft-365/admin/manage/remove-licenses-from-users) та [повторно призначте](/microsoft-365/admin/manage/assign-licenses-to-users) ліцензію Office, а потім [увійдіть в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9), використовуючи обліковий запис користувача.</span><span class="sxs-lookup"><span data-stu-id="4373c-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="4373c-116">Запустіть [Засіб вирішення проблем активації](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="4373c-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="4373c-117">Скиньте стан активації Office</span><span class="sxs-lookup"><span data-stu-id="4373c-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Скидання стану активації Office")
- [<span data-ttu-id="4373c-118">Виконайте відновлення з мережі для пакета Office</span><span class="sxs-lookup"><span data-stu-id="4373c-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="4373c-119">Додаткові способи виправлення неполадок див. в статтях:</span><span class="sxs-lookup"><span data-stu-id="4373c-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="4373c-120">Помилки про "неліцензований продукт" і помилки активації в Office</span><span class="sxs-lookup"><span data-stu-id="4373c-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="4373c-121">Помилка "На жаль, не вдалося підключитися до облікового запису. Спробуйте ще раз пізніше" під час активації Office</span><span class="sxs-lookup"><span data-stu-id="4373c-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)