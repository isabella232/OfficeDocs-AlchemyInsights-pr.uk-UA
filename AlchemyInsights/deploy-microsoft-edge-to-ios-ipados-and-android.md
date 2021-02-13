---
title: Розгортання Microsoft EDGE to iOS, iPadOS та Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194583"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="1e6c9-102">Розгортання Microsoft EDGE to iOS, iPadOS та Android</span><span class="sxs-lookup"><span data-stu-id="1e6c9-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="1e6c9-103">Наведений нижче сценарій, що керується нижче, допоможе вам призначати Microsoft EDGE користувачам iOS, iPadOS і пристроях Android.</span><span class="sxs-lookup"><span data-stu-id="1e6c9-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="1e6c9-104">Якщо ви заблокували користувачів із реєстрації мобільних пристроїв, цей сценарій не працюватиме, а користувачам знадобиться інсталювати Microsoft EDGE самостійно.</span><span class="sxs-lookup"><span data-stu-id="1e6c9-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="1e6c9-105">Під час керованого сценарію слід виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="1e6c9-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="1e6c9-106">Попередні вимоги</span><span class="sxs-lookup"><span data-stu-id="1e6c9-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="1e6c9-107">Введення</span><span class="sxs-lookup"><span data-stu-id="1e6c9-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="1e6c9-108">Основи</span><span class="sxs-lookup"><span data-stu-id="1e6c9-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="1e6c9-109">Конфігурації</span><span class="sxs-lookup"><span data-stu-id="1e6c9-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="1e6c9-110">Призначення</span><span class="sxs-lookup"><span data-stu-id="1e6c9-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="1e6c9-111">Рецензування та створення</span><span class="sxs-lookup"><span data-stu-id="1e6c9-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="1e6c9-112">Виконавши кроки, описані в керованих сценаріїв, політики Microsoft Inune дозволять використовувати наведені нижче функції Microsoft EDGE для бізнесу.</span><span class="sxs-lookup"><span data-stu-id="1e6c9-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="1e6c9-113">Подвійна ідентичність</span><span class="sxs-lookup"><span data-stu-id="1e6c9-113">Dual identity</span></span>
- <span data-ttu-id="1e6c9-114">Інтеграція з політикою захисту програми Microsoft Inune</span><span class="sxs-lookup"><span data-stu-id="1e6c9-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="1e6c9-115">Інтеграція з проксі-сервером застосунку «Лазурний активний каталог»</span><span class="sxs-lookup"><span data-stu-id="1e6c9-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="1e6c9-116">Ярлики керованих уподобань і домашньої сторінки</span><span class="sxs-lookup"><span data-stu-id="1e6c9-116">Managed favorites and home page shortcuts</span></span>
