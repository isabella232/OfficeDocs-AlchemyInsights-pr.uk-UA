---
title: Не вдається ввійти в Teams через помилку autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932284"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="fc182-102">Не вдається ввійти в Teams через помилку autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="fc182-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="fc182-103">Якщо як автентифікацію O365 увімкнуто функцію простого єдиного входу, можливо, до сайтів інтрамережі доведеться додати URL-адресу autologon.microsoftazuread-sso.com.</span><span class="sxs-lookup"><span data-stu-id="fc182-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="fc182-104">Якщо її вже додано до сайтів інтрамережі та використовується функція простого єдиного входу, вилучіть цю URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="fc182-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="fc182-105">Ознайомтеся з [контрольним списком із виправлення помилок простого єдиного входу](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="fc182-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="fc182-106">Щоб додати URL-адресу до списку сайтів інтрамережі, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="fc182-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="fc182-107">Відкрийте Internet Explorer, натиснувши кнопку **Пуск**.</span><span class="sxs-lookup"><span data-stu-id="fc182-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="fc182-108">У полі пошуку введіть Internet Explorer, а потім у списку результатів виберіть **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="fc182-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="fc182-109">Виберіть **Знаряддя**, а потім – **Властивості браузера**.</span><span class="sxs-lookup"><span data-stu-id="fc182-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="fc182-110">Перейдіть на вкладку **Безпека**.</span><span class="sxs-lookup"><span data-stu-id="fc182-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="fc182-111">Виберіть **Локальна інтрамережа**, натисніть кнопку **Сайти**, а потім – **Додатково**.</span><span class="sxs-lookup"><span data-stu-id="fc182-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="fc182-112">Введіть URL-адресу веб-сайту та виберіть **Додати**.</span><span class="sxs-lookup"><span data-stu-id="fc182-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="fc182-113">Після завершення натисніть кнопку **Закрити**.</span><span class="sxs-lookup"><span data-stu-id="fc182-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="fc182-114">Щоб отримати докладні відомості, див. статтю [Документація з розгортання функції простого єдиного входу для O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (містить інформацію про процес на основі політик, за допомогою якого можна додати URL-адресу до сайтів інтрамереж на кроці 3).</span><span class="sxs-lookup"><span data-stu-id="fc182-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
