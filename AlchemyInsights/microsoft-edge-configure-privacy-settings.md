---
title: Настроювання параметрів конфіденційності Microsoft EDGE
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678864"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="658cc-102">Настроювання параметрів конфіденційності Microsoft EDGE</span><span class="sxs-lookup"><span data-stu-id="658cc-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="658cc-103">За замовчуванням, якщо Microsoft EDGE розгорнуто на платформах, які не є ОС Windows, діагностичні дані та відомості про сайт не надсилатимуться до корпорації Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="658cc-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="658cc-104">Однак, якщо Microsoft EDGE розгорнуто в ОС Windows 10, діагностичні дані та відомості про сайт надсилатиметься відповідно до [параметрів діагностики даних Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="658cc-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="658cc-105">Ось як настроїти колекцію даних Microsoft EDGE для організації, використовуючи наведені нижче групові політики.</span><span class="sxs-lookup"><span data-stu-id="658cc-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="658cc-106">Параметри [метаданих](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ця політика дає змогу повідомляти про використання та дані, пов'язані з аварійними даними.</span><span class="sxs-lookup"><span data-stu-id="658cc-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="658cc-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ця політика надсилає відомості про сайт, які використовуються для вдосконалення служб Microsoft.</span><span class="sxs-lookup"><span data-stu-id="658cc-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="658cc-108">Докладні відомості наведено в статті [Настроювання параметрів політики](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="658cc-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>