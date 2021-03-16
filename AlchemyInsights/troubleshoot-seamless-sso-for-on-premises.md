---
title: Виправлення неполадок із надбудовами єдиного входу (SSO) для локального
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816345"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="22037-102">Виправлення неполадок із надбудовами єдиного входу (SSO) для локального</span><span class="sxs-lookup"><span data-stu-id="22037-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="22037-103">Щоб вирішити проблеми з невиконанням єдиного входу (SSO), виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="22037-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="22037-104">**Як можна пролонгувати ключ дешифрування для облікового запису AZUREADSSO на комп'ютері?**</span><span class="sxs-lookup"><span data-stu-id="22037-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="22037-105">Радимо, що ви обертаєте кілька ключів протоколу дешифрування принаймні кожні 30 днів.</span><span class="sxs-lookup"><span data-stu-id="22037-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="22037-106">Щоб виконати ці дії вручну, Дізнайтеся, як виконати перехід [за ключами дешифрування за протоколом Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="22037-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="22037-107">**Настроювання безшовного єдиного входу**</span><span class="sxs-lookup"><span data-stu-id="22037-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="22037-108">Щоб розгорнути безшовну службу ЄДИНОГО входу, виконайте дії, описані в надбудові " [Лазурний": "Швидкий запуск](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)".</span><span class="sxs-lookup"><span data-stu-id="22037-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="22037-109">**Рекомендації**</span><span class="sxs-lookup"><span data-stu-id="22037-109">**Advisory**</span></span>

- <span data-ttu-id="22037-110">Для єдиного входу в " [лазуровий":](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) запитання й відповіді – у цій статті наведено найпоширеніші запитання про Sign-On безшовну службу "Блакитний Active Directory" (БЕЗШОВНЕ SSO).</span><span class="sxs-lookup"><span data-stu-id="22037-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="22037-111">Знову стежте за новим вмістом.</span><span class="sxs-lookup"><span data-stu-id="22037-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="22037-112">[Microsoft Q&A-у](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) цій статті наведено відомості про те, як створювати запити на отримання функцій або задавати технічні запитання щодо БЕЗШОВНОГО входу.</span><span class="sxs-lookup"><span data-stu-id="22037-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="22037-113">**Виправлення неполадок**</span><span class="sxs-lookup"><span data-stu-id="22037-113">**Troubleshoot**</span></span>

<span data-ttu-id="22037-114">[Виправлення неполадок із єдиною надбудові "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) " – Ця стаття дає змогу знаходити відомості про виправлення неполадок із типовими відомостями про типові проблеми, пов'язані з однією Sign-On (БЕЗШОВНЕ єдиного входу).</span><span class="sxs-lookup"><span data-stu-id="22037-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







