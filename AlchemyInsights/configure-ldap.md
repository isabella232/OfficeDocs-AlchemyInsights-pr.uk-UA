---
title: Настроювання LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885582"
---
# <a name="configure-ldap"></a><span data-ttu-id="89445-102">Настроювання LDAP</span><span class="sxs-lookup"><span data-stu-id="89445-102">Configure LDAP</span></span>

<span data-ttu-id="89445-103">Щоб настроїти LDAP, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="89445-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="89445-104">Перевірте стан справності свого домену на [порталі Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="89445-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="89445-105">Переконайтеся, що доступна дійсна Передплата Azure AD, і служби "Лазурний домен AD" активовано.</span><span class="sxs-lookup"><span data-stu-id="89445-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="89445-106">Сертифікат, який потрібно ввімкнути для захищеного LDAP, має бути отримано з надійного центру сертифікації або бути сертифікатом, що самостійно підписано.</span><span class="sxs-lookup"><span data-stu-id="89445-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="89445-107">Переконайтеся, що сертифікат слід відповідно до потрібних [рекомендацій](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="89445-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="89445-108">**Неприпустимий сертифікат**</span><span class="sxs-lookup"><span data-stu-id="89445-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="89445-109">Щоб поновити сертифікат, дотримуйтеся вказівок, щоб створити новий сертифікат і повторно передати його: [НАСТРОЮВАННЯ LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="89445-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="89445-110">Щоб вирішити відому проблему з Захищенними оповіщеннями LDAP у службах домену Azure Active Directory, ознайомтеся з [вирішенням СПОВІЩЕНЬ LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="89445-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
