---
title: Microsoft Defender для кінцевої точки в Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731975"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="f08be-102">Microsoft Defender для кінцевої точки в Linux</span><span class="sxs-lookup"><span data-stu-id="f08be-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="f08be-103">Докладну документацію до Linux див. в статті [Microsoft Defender для кінцевої точки в Linux.](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux)</span><span class="sxs-lookup"><span data-stu-id="f08be-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="f08be-104">Відомості про систему та інсталяцію див. в такому:</span><span class="sxs-lookup"><span data-stu-id="f08be-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="f08be-105">Передумови</span><span class="sxs-lookup"><span data-stu-id="f08be-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="f08be-106">Системні вимоги</span><span class="sxs-lookup"><span data-stu-id="f08be-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="f08be-107">Інструкції з інсталяції</span><span class="sxs-lookup"><span data-stu-id="f08be-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="f08be-108">Мережеві підключення</span><span class="sxs-lookup"><span data-stu-id="f08be-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="f08be-109">Інструкції див. в наведених нижче вказівках.</span><span class="sxs-lookup"><span data-stu-id="f08be-109">For instructions, see:</span></span>

- [<span data-ttu-id="f08be-110">Настроювання проксі-сервера пристрою та параметрів підключення до Інтернету</span><span class="sxs-lookup"><span data-stu-id="f08be-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="f08be-111">Розгортання оновлень для кінцевої точки Для Захисника Microsoft у Linux</span><span class="sxs-lookup"><span data-stu-id="f08be-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="f08be-112">Налаштування програми "Захисник Microsoft" для кінцевої точки в Linux</span><span class="sxs-lookup"><span data-stu-id="f08be-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="f08be-113">Підтримувані команди</span><span class="sxs-lookup"><span data-stu-id="f08be-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="f08be-114">Мені потрібна допомога!</span><span class="sxs-lookup"><span data-stu-id="f08be-114">I need help!</span></span>

<span data-ttu-id="f08be-115">Якщо не вдається знайти потрібну інформацію або довідку, увімкніться пошук.</span><span class="sxs-lookup"><span data-stu-id="f08be-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="f08be-116">Перш ніж звернутися до служби підтримки Microsoft, обов'язково зберіть дані, необхідні, щоб з'ясувати причину проблеми, і прикріпіть їх до запиту.</span><span class="sxs-lookup"><span data-stu-id="f08be-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="f08be-117">Інструкції з збирання діагностичних відомостей див. в [статті Збирання діагностичних даних.](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information)</span><span class="sxs-lookup"><span data-stu-id="f08be-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>