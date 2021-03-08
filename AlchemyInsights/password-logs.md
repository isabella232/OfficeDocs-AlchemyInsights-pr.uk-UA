---
title: Журнали паролів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527775"
---
# <a name="password-logs"></a><span data-ttu-id="14710-102">Журнали паролів</span><span class="sxs-lookup"><span data-stu-id="14710-102">Password logs</span></span>

<span data-ttu-id="14710-103">**Проблеми з доступом до журналів аудиту скидання пароля**</span><span class="sxs-lookup"><span data-stu-id="14710-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="14710-104">Щоб вирішити проблеми, пов'язані з доступом до журналів аудиту для скидання пароля, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="14710-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="14710-105">Переконайтеся, що ви маєте право переглядати журнали аудиту.</span><span class="sxs-lookup"><span data-stu-id="14710-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="14710-106">Авторизовані лише такі ролі:</span><span class="sxs-lookup"><span data-stu-id="14710-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="14710-107">Глобальний адміністратор</span><span class="sxs-lookup"><span data-stu-id="14710-107">Global administrator</span></span>
 - <span data-ttu-id="14710-108">Адміністратор системи безпеки</span><span class="sxs-lookup"><span data-stu-id="14710-108">Security administrator</span></span>
 - <span data-ttu-id="14710-109">Читач безпеки</span><span class="sxs-lookup"><span data-stu-id="14710-109">Security reader</span></span>

<span data-ttu-id="14710-110">**Я хочу Переглянути всі події перевірки скидання пароля з моменту, коли ви спочатку розгорнули**</span><span class="sxs-lookup"><span data-stu-id="14710-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="14710-111">За останні 30 днів у звітах про зміни пароля та реєстраційних подій 120 000 зберігаються.</span><span class="sxs-lookup"><span data-stu-id="14710-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="14710-112">Цей максимальний ліміт застосовується до інтерфейсу користувача під час завантаження файлу CSV.</span><span class="sxs-lookup"><span data-stu-id="14710-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="14710-113">події 1 000 000 доступні за допомогою PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14710-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="14710-114">Щоб отримати докладніші відомості, ознайомтеся з наведеними нижче посиланнями.</span><span class="sxs-lookup"><span data-stu-id="14710-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="14710-115">Повідомлення про те, що для самостійного скидання пароля з неавтоматичної служби й API подій</span><span class="sxs-lookup"><span data-stu-id="14710-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="14710-116">Швидке завантаження подій для реєстрації паролів швидко за допомогою PowerShell</span><span class="sxs-lookup"><span data-stu-id="14710-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="14710-117">**Я хочу дізнатися більше про можливості звітування про скидання пароля**</span><span class="sxs-lookup"><span data-stu-id="14710-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="14710-118">Перевірка користувачів, які реєструють або скиньте паролі за допомогою журналів аудиту Azure AD для скидання пароля на порталі "Лазурний" в розділі " **користувачі та групи**".</span><span class="sxs-lookup"><span data-stu-id="14710-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="14710-119">Щоб отримати докладніші відомості, ознайомтеся з такими посиланнями:</span><span class="sxs-lookup"><span data-stu-id="14710-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="14710-120">Огляд звітів про скидання пароля</span><span class="sxs-lookup"><span data-stu-id="14710-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="14710-121">Перегляд звітів про скидання пароля на порталі «Лазурний»</span><span class="sxs-lookup"><span data-stu-id="14710-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="14710-122">Повідомлення про те, що для самостійного скидання пароля з неавтоматичної служби й API подій</span><span class="sxs-lookup"><span data-stu-id="14710-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="14710-123">Швидке завантаження подій для реєстрації паролів швидко за допомогою PowerShell</span><span class="sxs-lookup"><span data-stu-id="14710-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


