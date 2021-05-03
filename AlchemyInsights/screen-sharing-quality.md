---
title: Якість спільного доступу до екрана
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125769"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="11d20-102">Якість спільного доступу до екрана</span><span class="sxs-lookup"><span data-stu-id="11d20-102">Screen sharing quality</span></span>

<span data-ttu-id="11d20-103">У більшості випадків проблеми з якістю спільного доступу до екрана знизя до обмеженої смуги пропускання з боку клієнта.</span><span class="sxs-lookup"><span data-stu-id="11d20-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="11d20-104">Якщо смуга пропускання не обмежена, у програмі Teams оптимізується якість мультимедіа, зокрема роздільна здатність відео до 1080p, до 30fps для відео та 15fps для вмісту та високоякісне аудіо.</span><span class="sxs-lookup"><span data-stu-id="11d20-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="11d20-105">Teams завжди консервативний під час утилізації смуги пропускання та може забезпечувати якість відео у форматі HD із роздільною здатністю до 1,2 Мбіт/с.</span><span class="sxs-lookup"><span data-stu-id="11d20-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="11d20-106">Фактичне споживання смуги пропускання для кожного аудіо- чи відеовиклику або наради за різною роботою залежно від таких факторів, як макет відео, роздільна здатність відео та рамки відео за секунду.</span><span class="sxs-lookup"><span data-stu-id="11d20-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="11d20-107">Коли доступна більша смуга пропускання, якість і використання збільшаться, щоб підвищити ефективність роботи.</span><span class="sxs-lookup"><span data-stu-id="11d20-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="11d20-108">У цій таблиці описано, як Teams використовувати смугу пропускання:</span><span class="sxs-lookup"><span data-stu-id="11d20-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="11d20-109">**Сценарії смуги пропускання (угору та вниз)**</span><span class="sxs-lookup"><span data-stu-id="11d20-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="11d20-110">30 кбіт/с під час аудіовиклику</span><span class="sxs-lookup"><span data-stu-id="11d20-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="11d20-111">130 кбіт/с для однорангих аудіовиклику та спільний перегляд екрана</span><span class="sxs-lookup"><span data-stu-id="11d20-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="11d20-112">Відеовиклик 360p із частотою 500 кбіт/с</span><span class="sxs-lookup"><span data-stu-id="11d20-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="11d20-113">1,2 Мбіт/с для відеовиклику в однократному форматі HD із роздільною здатністю HD 720p для 30fps</span><span class="sxs-lookup"><span data-stu-id="11d20-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="11d20-114">1,5 Мбіт/с для відеовиклику в однократному форматі HD із роздільною здатністю HD 1080p для 30fps</span><span class="sxs-lookup"><span data-stu-id="11d20-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="11d20-115">500 кбіт/с; групові відеовиклики</span><span class="sxs-lookup"><span data-stu-id="11d20-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="11d20-116">1 Мбіт/с; 2 Мбіт/с для відеовикликів у форматі HD (відео в режимі 540p на екрані 1080p)</span><span class="sxs-lookup"><span data-stu-id="11d20-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="11d20-117">Докладні відомості див. [в розділі Підготовка мережі організації до Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="11d20-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>