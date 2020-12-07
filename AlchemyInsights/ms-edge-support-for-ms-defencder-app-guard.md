---
title: Підтримка Microsoft EDGE для охоронця програм Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584006"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="fbdac-102">Підтримка Microsoft EDGE для охоронця програм Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="fbdac-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="fbdac-103">Для Windows 10 і Microsoft EDGE програма Guard використовує апаратно-ізольований підхід, який дає змогу користувачам переходити від ненадійного сайту в ізольованому, гіпер-V – контейнері, відокремленому від операційної системи хоста.</span><span class="sxs-lookup"><span data-stu-id="fbdac-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="fbdac-104">Адміністратор підприємства визначає список надійних веб-сайтів, хмарних ресурсів і внутрішніх мереж.</span><span class="sxs-lookup"><span data-stu-id="fbdac-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="fbdac-105">Коли користувач відвідує сайт, який немає в списку, Microsoft EDGE відкриє сайт в контейнері.</span><span class="sxs-lookup"><span data-stu-id="fbdac-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="fbdac-106">Це означає, що якщо сайт стане зловмисним, хост-ПК залишиться захищеним, а зловмисник не отримає корпоративні дані.</span><span class="sxs-lookup"><span data-stu-id="fbdac-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="fbdac-107">Інсталяція розширень у контейнері підтримується як Microsoft EDGE Version 81, і його можна керувати за допомогою політики.</span><span class="sxs-lookup"><span data-stu-id="fbdac-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="fbdac-108">Адреса Updationeurl, що використовується в політиці розширення, має бути доданий як нейтральний ресурс у політиці мережної ізоляції, що використовується програмою "охоронець".</span><span class="sxs-lookup"><span data-stu-id="fbdac-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="fbdac-109">Докладні відомості наведено в статті [підтримка Microsoft EDGE для охоронця програм Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="fbdac-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
