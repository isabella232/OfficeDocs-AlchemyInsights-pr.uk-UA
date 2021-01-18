---
title: Віртуальна конфігурація з службами доменів AAD
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
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885654"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="22660-102">Віртуальна конфігурація з службами доменів AAD</span><span class="sxs-lookup"><span data-stu-id="22660-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="22660-103">Віртуальна конфігурація з службами доменів AAD включає наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="22660-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="22660-104">Перевірка справності вашого домену на порталі «Лазурний» https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="22660-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="22660-105">Перевірка НСГ для правил, які блокують порти, необхідні для синхронізації в службі "Azure domain AD" на порталі https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="22660-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="22660-106">Переконайтеся, що віртуальну мережу розгорнуто в тій самій Лазужній області, як-от домен Azure AD служби доменів.</span><span class="sxs-lookup"><span data-stu-id="22660-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="22660-107">Переконайтеся, що у вас немає наявного домену з таким самим іменем домену, доступним у віртуальній мережі.</span><span class="sxs-lookup"><span data-stu-id="22660-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="22660-108">Щоб отримати докладні відомості про розгляд у віртуальній мережі Azure Virtual Network для підтримки служб домену AAD, ознайомтеся з відомостями про [віртуальну мережу](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="22660-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

