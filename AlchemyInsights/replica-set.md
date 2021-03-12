---
title: Набір реплік
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714588"
---
# <a name="replica-set"></a><span data-ttu-id="b577c-102">Набір реплік</span><span class="sxs-lookup"><span data-stu-id="b577c-102">Replica set</span></span>

<span data-ttu-id="b577c-103">AADDS також називають керованим доменом.</span><span class="sxs-lookup"><span data-stu-id="b577c-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="b577c-104">Це насправді два контролери домену, які виконуються й підтримуються на внутрішньому сервері.</span><span class="sxs-lookup"><span data-stu-id="b577c-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="b577c-105">Два ЦСК включають один основний DC і один реплікацію DC.</span><span class="sxs-lookup"><span data-stu-id="b577c-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="b577c-106">Резервне копіювання в надбудові AADDS (керований домен) – це автоматизований процес, керований платформою Azure.</span><span class="sxs-lookup"><span data-stu-id="b577c-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="b577c-107">У разі проблеми з керованим доменом, підтримка Azure може допомогти вам відновити роботу з резервної копії.</span><span class="sxs-lookup"><span data-stu-id="b577c-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="b577c-108">Ви створюєте набір реплік у віртуальній мережі.</span><span class="sxs-lookup"><span data-stu-id="b577c-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="b577c-109">Кожна віртуальна мережа має бути в кожній іншій віртуальній мережі, де розміщено набір реплік керованого домену.</span><span class="sxs-lookup"><span data-stu-id="b577c-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="b577c-110">Ця конфігурація створює топологію мережі сітки, яка підтримує реплікацію каталогів.</span><span class="sxs-lookup"><span data-stu-id="b577c-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="b577c-111">Віртуальна мережа може підтримувати кілька наборів реплік, за умови, що кожний набір реплік перебуває в іншій віртуальній підмережі.</span><span class="sxs-lookup"><span data-stu-id="b577c-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="b577c-112">Докладні відомості про набір реплік наведено в статті [Набори реплік "концепції](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)".</span><span class="sxs-lookup"><span data-stu-id="b577c-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
