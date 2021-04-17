---
title: Центр адміністрування Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826400"
---
# <a name="teams-admin-center"></a><span data-ttu-id="4343f-102">Центр адміністрування Teams</span><span class="sxs-lookup"><span data-stu-id="4343f-102">Teams Admin Center</span></span>

<span data-ttu-id="4343f-103">Дізнайтеся, як керувати Teams за допомогою [Центру адміністрування Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4343f-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="4343f-104">Якщо вам не вдається отримати доступ до Центру адміністрування Teams, виконайте наведені нижче вказівки.</span><span class="sxs-lookup"><span data-stu-id="4343f-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="4343f-105">Пересвідчіться, що ви надали дозволи відповідним [IP- та URL-адресам Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всіх пристроях захисту мережевого периметра (брандмауер тощо) або в правилах брандмауера на локальному комп’ютері.</span><span class="sxs-lookup"><span data-stu-id="4343f-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="4343f-106">Переконайтеся, що логін, який використовується, щоб отримати доступ до порталу адміністрування Teams, відповідає вашому імені користувача, вказаним на [порталі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="4343f-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="4343f-107">Якщо користувачі не відображаються в центрі адміністрування Teams, перевірте вказане нижче.</span><span class="sxs-lookup"><span data-stu-id="4343f-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="4343f-108">Ви створювали користувачів або призначали ліцензії протягом останніх 24 годин?</span><span class="sxs-lookup"><span data-stu-id="4343f-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="4343f-109">Перш ніж відкрити квиток підтримки, переконайтеся, що минуло принаймні 24 години.</span><span class="sxs-lookup"><span data-stu-id="4343f-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="4343f-110">Пересвідчіться, що ви призначили відповідні ліцензії.</span><span class="sxs-lookup"><span data-stu-id="4343f-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="4343f-111">Якщо у вас є локальна служба Active Directory, переконайтеся, що значення [msRTCSIP-PrimaryUserAddress або SIP-адреси в полі ProxyAddresses](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) у локальній службі Active Directory унікальне, а формат відповідає sip: ім'я користувача з Центру адміністрування Microsoft [365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="4343f-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="4343f-112">Якщо ви планували зберегти розгортання "Skype для бізнесу – сервер" і розгорнути їх у локальному середовищі та онлайн, виконайте вказівки "Налаштування гібридного розгортання з Teams і "Skype для бізнесу – онлайн" на Панелі керування "Skype для бізнесу – **сервер"** і перемістіть користувачів через Інтернет.</span><span class="sxs-lookup"><span data-stu-id="4343f-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
