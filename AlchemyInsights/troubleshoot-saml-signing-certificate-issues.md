---
title: Виправлення неполадок із сертифікатом для підпису в SAML
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
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694454"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="376e8-102">Виправлення неполадок із сертифікатом для підпису в SAML</span><span class="sxs-lookup"><span data-stu-id="376e8-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="376e8-103">Щоб вирішити проблему сертифіката підпису, виконайте наведені нижче Рекомендовані дії.</span><span class="sxs-lookup"><span data-stu-id="376e8-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="376e8-104">Під час додавання корпоративної програми, яка підтримує SSO, Azure створить сертифікат, який називається [сертифікатом підпису SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="376e8-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="376e8-105">Цей сертифікат має термін дії 3 роки.</span><span class="sxs-lookup"><span data-stu-id="376e8-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="376e8-106">Щоб змінити дату завершення терміну дії сертифіката, перегляньте статтю [Настроювання дати завершення терміну дії сертифіката Федерації та прокрутіть його до нового сертифіката](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="376e8-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="376e8-107">За допомогою цього сертифіката буде використано цей сертифікат, щоб підписати маркери SAML, які просили програма, і відправить його до програми для успішного входу.</span><span class="sxs-lookup"><span data-stu-id="376e8-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="376e8-108">Щоб виконати цю дію, завантажте сертифікат із порталу "Лазурний" та відправте його постачальнику програм, щоб завершити процес єдиного входу.</span><span class="sxs-lookup"><span data-stu-id="376e8-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="376e8-109">Після завершення цього процесу програма буде довіряти цьому сертифікату, і всі маркери SAML, підписані цим сертифікатом, прийматимуться програмою.</span><span class="sxs-lookup"><span data-stu-id="376e8-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="376e8-110">Якщо термін дії цього сертифіката завершився, створіть новий сертифікат, оновіть її до постачальника програм, а потім зробіть його активним на Лазурому боці.</span><span class="sxs-lookup"><span data-stu-id="376e8-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="376e8-111">Щоб отримати додаткові відомості, перегляньте статтю [поновити сертифікат, який незабаром завершиться](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="376e8-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="376e8-112">Якщо сертифікат завершується, користувач не заблокуватиметься.</span><span class="sxs-lookup"><span data-stu-id="376e8-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="376e8-113">[Додайте адресу електронної пошти для сповіщень](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , які потрібно отримати, перш ніж закінчиться термін дії поточного сертифіката.</span><span class="sxs-lookup"><span data-stu-id="376e8-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="376e8-114">Крок – 4 – необов'язковий.</span><span class="sxs-lookup"><span data-stu-id="376e8-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="376e8-115">Змінення параметрів підпису сертифіката в програмі SAML і алгоритм підпису сертифіката.</span><span class="sxs-lookup"><span data-stu-id="376e8-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="376e8-116">Докладні відомості наведено в статті [змінення параметрів підпису сертифіката та алгоритму підпису](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="376e8-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

