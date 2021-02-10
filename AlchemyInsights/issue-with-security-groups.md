---
title: Проблема з групами безпеки
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177637"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="bd3d6-102">Проблема з групами безпеки</span><span class="sxs-lookup"><span data-stu-id="bd3d6-102">Issue with security groups</span></span>

<span data-ttu-id="bd3d6-103">**Якщо ви одержуєте помилки в мережі AADDS104**</span><span class="sxs-lookup"><span data-stu-id="bd3d6-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="bd3d6-104">Неприпустимі правила групи безпеки мережі – це найпоширеніша причина помилок мережі для служб домену Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="bd3d6-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="bd3d6-105">Група безпеки мережі для віртуальної мережі має дозволити доступ до певних портів і протоколів.</span><span class="sxs-lookup"><span data-stu-id="bd3d6-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="bd3d6-106">Якщо ці порти блокуються, платформа Azure не може відстежувати або оновлювати керований домен.</span><span class="sxs-lookup"><span data-stu-id="bd3d6-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="bd3d6-107">Це також впливає на синхронізацію між Лазуроним оголошенням і Лазуроним ОГОЛОШЕННЯМ DS.</span><span class="sxs-lookup"><span data-stu-id="bd3d6-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="bd3d6-108">Переконайтеся, що ви зберігаєте відкриті порти за замовчуванням, щоб уникнути переривання обслуговування.</span><span class="sxs-lookup"><span data-stu-id="bd3d6-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="bd3d6-109">Щоб зрозуміти та вирішити поширені проблеми з конфігурацією мережної системи безпеки, перегляньте статтю [Додавання та перевірка груп безпеки](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="bd3d6-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
