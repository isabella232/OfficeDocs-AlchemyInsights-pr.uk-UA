---
title: Не працює з Wriтиповернення пароля
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243731"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="b8801-102">Не працює з Wriтиповернення пароля</span><span class="sxs-lookup"><span data-stu-id="b8801-102">Password Writeback is not working</span></span>

<span data-ttu-id="b8801-103">**У мене виникли проблеми з настроюванням запису пароля**</span><span class="sxs-lookup"><span data-stu-id="b8801-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="b8801-104">Password wriтиback – це Преміальний компонент.</span><span class="sxs-lookup"><span data-stu-id="b8801-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="b8801-105">Переконайтеся, що ви зрозуміли вимоги до ліцензування:</span><span class="sxs-lookup"><span data-stu-id="b8801-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="b8801-106">Потрібно мати принаймні одну ліцензію, призначену в організації</span><span class="sxs-lookup"><span data-stu-id="b8801-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="b8801-107">**Хмарні тільки користувачі** – будь-який Office 365 (O365) платний обліковий номер або ЛАЗУРНЕ AD Basic</span><span class="sxs-lookup"><span data-stu-id="b8801-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="b8801-108">**Хмарні та/або Локальні користувачі** – AZURE AD Premium P1 або P2, Enterprise Mobility + Security (EMS) або захищене продуктивне підприємство (SPE).</span><span class="sxs-lookup"><span data-stu-id="b8801-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="b8801-109">Додаткові відомості про вимоги до ліцензування наведено в статті [вимоги до ліцензування для скидання пароля служби самообслуговування Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) .</span><span class="sxs-lookup"><span data-stu-id="b8801-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="b8801-110">У вас є принаймні один обліковий запис адміністратора, а один тестовий обліковий запис користувача з однією з відповідної ліцензії.</span><span class="sxs-lookup"><span data-stu-id="b8801-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="b8801-111">Ви повинні підключити Azure AD Connect до головного емулятора контролера домену для wriveback для роботи з паролем.</span><span class="sxs-lookup"><span data-stu-id="b8801-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="b8801-112">Ви можете налаштувати Azure AD Connect для використання основного контролера домену, клацнувши правою кнопкою миші **Властивості** сполучної лінії синхронізації Active Directory, а потім виберіть пункт **настроїти розділи каталогів**.</span><span class="sxs-lookup"><span data-stu-id="b8801-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="b8801-113">Звідти знайдіть розділ **Параметри підключення контролера домену** та установіть прапорець **використовувати лише контролери домену**.</span><span class="sxs-lookup"><span data-stu-id="b8801-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="b8801-114">Якщо перевага для постійного струму не є емулятором PDC, то "Azure AD Connect" все одно буде досягнуто в службі PDC для визначення пароля.</span><span class="sxs-lookup"><span data-stu-id="b8801-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="b8801-115">Скидання пароля настроєно та ввімкнуто в клієнті.</span><span class="sxs-lookup"><span data-stu-id="b8801-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="b8801-116">Щоб отримати докладніші відомості, Дізнайтеся, як [дозволити користувачам скинути їхні паролі Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="b8801-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="b8801-117">Переконайтеся, що обліковий запис адміністратора, який використовується для того, щоб увімкнути Wriтиback – обліковий запис адміністратора хмари (створений у Лазурому, не локальний РЕКЛАМНИЙ)</span><span class="sxs-lookup"><span data-stu-id="b8801-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="b8801-118">У вас є один або кілька лісових ОБ'ЯВ локального розгортання під керуванням Windows Server 2008 R2, Windows Server 2012 або Windows Server 2012 R2 з найновішими інстальованими пакетами оновлень</span><span class="sxs-lookup"><span data-stu-id="b8801-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="b8801-119">У вас інстальовано засіб Azure AD Connect, і ви підготували середовище для синхронізації до хмари.</span><span class="sxs-lookup"><span data-stu-id="b8801-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="b8801-120">Перш ніж протестувати пароль writeback, переконайтеся, що спочатку потрібно виконати повне імпортування та повну синхронізацію з AD і Azure AD Connect Azure.</span><span class="sxs-lookup"><span data-stu-id="b8801-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="b8801-121">Дізнайтеся більше про те, як виконати [повну синхронізацію та повний імпорт у лазурому для підключення до мережі](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="b8801-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="b8801-122">**У мене виникли проблеми з підключенням до wriтиповернення пароля**</span><span class="sxs-lookup"><span data-stu-id="b8801-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="b8801-123">Завантажте та активуйте найновішу версію служби [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="b8801-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="b8801-124">Конфігурація брандмауера: засіб Azure AD Connect (1.1.443 і вище) матиме доступ до **ВИХІДНОГО HTTPS** :</span><span class="sxs-lookup"><span data-stu-id="b8801-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="b8801-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b8801-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="b8801-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="b8801-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="b8801-127">Дозволити простоювання підключень протягом щонайменше 2-3 хвилин</span><span class="sxs-lookup"><span data-stu-id="b8801-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="b8801-128">**У мене все ще виникають проблеми з wriтиповернення пароля**</span><span class="sxs-lookup"><span data-stu-id="b8801-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="b8801-129">Якщо ви все ще відчуваєте труднощі, скористайтеся вимкненням та повторно активованою службою wriveback для використання в засобі створення Лазурової програми AD Connect</span><span class="sxs-lookup"><span data-stu-id="b8801-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="b8801-130">Щоб дізнатися більше, Дізнайтеся більше про те, як [Вимкнути та знову ввімкнути wriтиповернутися паролем](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="b8801-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
