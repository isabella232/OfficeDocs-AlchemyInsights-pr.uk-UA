---
title: Контролер домену
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901318"
---
# <a name="domain-controller"></a><span data-ttu-id="85015-102">Контролер домену</span><span class="sxs-lookup"><span data-stu-id="85015-102">Domain controller</span></span>

<span data-ttu-id="85015-103">**Не вдається ввімкнути AAD-DS або розгортання не вдається**</span><span class="sxs-lookup"><span data-stu-id="85015-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="85015-104">Щоб вирішити проблему, яка не активується (AAD-DS) не ввімкнуто або не вдається розгорнути, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="85015-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="85015-105">Якщо ви використовуєте вже наявну віртуальну мережу, перевірте свої правила, які блокують порти, необхідні для синхронізації в AAD-DS на порталі https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="85015-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="85015-106">Перевірте, чи відповідь на повідомлення про помилку в цьому посібнику з виправлення неполадок, доступний у програмі  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="85015-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="85015-107">У новій віртуальній мережі можна виконати розгортання служб для домену Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85015-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="85015-108">Виконайте посібник із початку роботи, щоб розгорнути AAD-DS, який можна отримати в [Посібнику з створення служб домену Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="85015-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="85015-109">Якщо у вас виникли проблеми з розгортанням служб домену Azure AD, перегляньте статтю [Виправлення неполадок служби "Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) " для вирішення поширених помилок, щоб допомогти вам знову працювати з ними.</span><span class="sxs-lookup"><span data-stu-id="85015-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="85015-110">**Не вдається вимкнути AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="85015-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="85015-111">AAD-DS не може бути призупинено.</span><span class="sxs-lookup"><span data-stu-id="85015-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="85015-112">Якщо ви хочете припинити використовувати керований домен, його потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="85015-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="85015-113">Якщо ви зіткнулися з проблемами, щоб вирішити поширені повідомлення про помилки, а також пов'язані з ними кроки з виправлення неполадок, щоб допомогти вам знову працювати з ними, ознайомтеся з [усуненням служб домену "Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)"</span><span class="sxs-lookup"><span data-stu-id="85015-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
