---
title: Сповіщення про підключення до AAD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037232"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="83e18-102">Сповіщення про підключення до AAD</span><span class="sxs-lookup"><span data-stu-id="83e18-102">Notification AAD Connect</span></span>

- <span data-ttu-id="83e18-103">Переконайтеся, що ви маєте право виконати операцію.</span><span class="sxs-lookup"><span data-stu-id="83e18-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="83e18-104">Глобальні адміністратори мають доступ за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="83e18-104">Global Admins have access by default.</span></span> <span data-ttu-id="83e18-105">Крім того, можна використовувати [елемент керування доступом на основі ролей](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , щоб отримати дозвіл на реєстрацію представника.</span><span class="sxs-lookup"><span data-stu-id="83e18-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="83e18-106">Переконайтеся, що потрібні кінцеві точки ввімкнуто, а не заблоковано через брандмауер.</span><span class="sxs-lookup"><span data-stu-id="83e18-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="83e18-107">Докладні відомості наведено в статті [вимоги](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="83e18-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="83e18-108">Реєстрація може не відповідно до вихідних повідомлень, які піддаються перевірці SSL через мережевий рівень.</span><span class="sxs-lookup"><span data-stu-id="83e18-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="83e18-109">Переконайтеся, що ви перевірили параметри сповіщень для служби "Azure AD Connect Health" і перегляньте свій параметр.</span><span class="sxs-lookup"><span data-stu-id="83e18-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="83e18-110">Щоб зрозуміти, як настроїти параметри сповіщень для сповіщень про справність служби Azure AD Connect, перегляньте цей [посібник](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="83e18-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="83e18-111">Щоб дізнатися більше про звіт про синхронізацію служби AAD Connect, а також про те, як завантажити його, перегляньте статтю [звіт про синхронізацію на рівні об'єкта](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="83e18-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="83e18-112">Щоб виправити неполадки з оповіщення про справність AAD Connect, виконайте вказівки [з виправлення неполадок для сповіщень про стан справності та відповіді](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) на поширені запитання в розділі [Загальні запитання про інсталяцію СПРАВНОСТІ служби aad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="83e18-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
