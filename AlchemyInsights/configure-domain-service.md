---
title: Настроювання служби доменів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885683"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="104b7-102">Не вдається ввімкнути AAD-DS або розгортання не вдається</span><span class="sxs-lookup"><span data-stu-id="104b7-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="104b7-103">Щоб вирішити проблему, яка не активується (AAD-DS) не ввімкнуто або не вдається розгорнути, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="104b7-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="104b7-104">Якщо ви використовуєте вже наявну віртуальну мережу, перевірте свої правила, які блокують порти, необхідні для синхронізації в AAD-DS на порталі https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="104b7-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="104b7-105">Перевірте, чи відповідь на повідомлення про помилку в цьому посібнику з виправлення неполадок, доступний у програмі  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="104b7-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="104b7-106">У новій віртуальній мережі можна виконати розгортання служб для домену Azure AD.</span><span class="sxs-lookup"><span data-stu-id="104b7-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="104b7-107">Виконайте інструкції з початку роботи з розгортання AAD-DS: [створення та настроювання служб ДОМЕНУ aad](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="104b7-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="104b7-108">Якщо у вас виникли проблеми з розгортанням служб домену Azure AD, перегляньте статтю [Виправлення неполадок служби "Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) " для вирішення поширених помилок, щоб допомогти вам знову працювати з ними.</span><span class="sxs-lookup"><span data-stu-id="104b7-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="104b7-109">**Не вдається вимкнути AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="104b7-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="104b7-110">AAD-DS не може бути призупинено.</span><span class="sxs-lookup"><span data-stu-id="104b7-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="104b7-111">Якщо ви хочете припинити використовувати керований домен, його потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="104b7-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="104b7-112">Щоб видалити керований домен, ознайомтеся з елементом [Видалити службу доменів AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="104b7-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



