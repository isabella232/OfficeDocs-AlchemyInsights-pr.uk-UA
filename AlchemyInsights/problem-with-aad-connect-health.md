---
title: Проблема зі здоров'ям AAD Connect
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483124"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="fe6a3-102">Проблема зі здоров'ям AAD Connect</span><span class="sxs-lookup"><span data-stu-id="fe6a3-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="fe6a3-103">Переконайтеся, що ви маєте право виконати операцію.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fe6a3-104">Глобальні адміністратори мають доступ за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-104">Global Admins have access by default.</span></span> <span data-ttu-id="fe6a3-105">Крім того, можна використовувати [елемент керування доступом на основі ролей](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , щоб отримати дозвіл на реєстрацію представника.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fe6a3-106">Переконайтеся, що потрібні кінцеві точки ввімкнуто, а не заблоковано через брандмауер.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fe6a3-107">Докладні відомості наведено в статті [вимоги](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="fe6a3-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fe6a3-108">Реєстрація може не відповідно до вихідних повідомлень, які піддаються перевірці SSL через мережевий рівень.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fe6a3-109">Переконайтеся, що ви підтвердили параметри сповіщень для справності для Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="fe6a3-110">Ознайомтеся з вашим параметром.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-110">Please review your setting.</span></span> <span data-ttu-id="fe6a3-111">Цей [посібник](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) допоможе вам дізнатися, як настроїти параметри сповіщень для сповіщень про справність служби AZURE AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fe6a3-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="fe6a3-112">Щоб дізнатися більше про звіт про синхронізацію служби AAD Connect, а також про те, як завантажити його, перегляньте статтю [звіт про синхронізацію на рівні об'єкта](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="fe6a3-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fe6a3-113">Щоб виправити неполадки з оповіщеннями в службі AAD Connect для справності, виконайте вказівки [з виправлення неполадок для сповіщень про стан справності та відповіді](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) на поширені запитання в розділі [Загальні запитання про інсталяцію СПРАВНОСТІ служби aad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="fe6a3-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
