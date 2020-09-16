---
title: Центр адміністрування Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670385"
---
# <a name="teams-admin-center"></a><span data-ttu-id="a0b98-102">Центр адміністрування Teams</span><span class="sxs-lookup"><span data-stu-id="a0b98-102">Teams Admin Center</span></span>

<span data-ttu-id="a0b98-103">Дізнайтеся, як керувати Teams за допомогою [Центру адміністрування Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a0b98-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="a0b98-104">Якщо вам не вдається отримати доступ до Центру адміністрування Teams, виконайте наведені нижче вказівки.</span><span class="sxs-lookup"><span data-stu-id="a0b98-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="a0b98-105">Пересвідчіться, що ви надали дозволи відповідним [IP- та URL-адресам Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всіх пристроях захисту мережевого периметра (брандмауер тощо) або в правилах брандмауера на локальному комп’ютері.</span><span class="sxs-lookup"><span data-stu-id="a0b98-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="a0b98-106">Переконайтеся, що логін, який використовується, щоб отримати доступ до порталу адміністрування Teams, відповідає вашому імені користувача, вказаним на [порталі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a0b98-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="a0b98-107">Якщо користувачі не відображаються в центрі адміністрування Teams, перевірте вказане нижче.</span><span class="sxs-lookup"><span data-stu-id="a0b98-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="a0b98-108">Ви створювали користувачів або призначали ліцензії протягом останніх 24 годин?</span><span class="sxs-lookup"><span data-stu-id="a0b98-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="a0b98-109">Перш ніж відкрити квиток підтримки, переконайтеся, що минуло принаймні 24 години.</span><span class="sxs-lookup"><span data-stu-id="a0b98-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="a0b98-110">Пересвідчіться, що ви призначили відповідні ліцензії.</span><span class="sxs-lookup"><span data-stu-id="a0b98-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="a0b98-111">Якщо у вас є локальна Служба Active Directory, переконайтеся, що [значення параметра msRTCSIP-PrimaryUserAddress або SIP-адреса в полі "proxyAddress" в локальному Active Directory є унікальним, а формат відповідає](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**ім'я** користувача в [центрі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a0b98-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="a0b98-112">Якщо ви збираєтесь зберегти розгортання на сервері Skype для бізнесу, а також користувачі, які створили локальну та онлайнове повідомлення, виконайте **команду "Настроювання гібридного використання команд і" Skype для бізнесу – онлайн "** на панелі керування служби" Skype для бізнесу "та перенесіть користувачів в онлайні.</span><span class="sxs-lookup"><span data-stu-id="a0b98-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
