---
title: Налаштування параметрів конфіденційності в Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405728"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="b056f-102">Налаштування параметрів конфіденційності в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b056f-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="b056f-103">За замовчуванням, якщо Microsoft Edge розгортаються на платформах, крім Windows, діагностичні дані та відомості про сайт не надсилаються до корпорації Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b056f-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="b056f-104">Однак якщо Microsoft Edge розгорнуто у Windows 10, діагностичні дані та відомості про сайт надсилаються відповідно до настройок діагностичних [даних Windows користувачів](https://go.microsoft.com/fwlink/?linkid=2132472).</span><span class="sxs-lookup"><span data-stu-id="b056f-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="b056f-105">Щоб налаштувати спосіб обробки даних в організації в Microsoft Edge, скористайтеся наведеними нижче груповими політиками.</span><span class="sxs-lookup"><span data-stu-id="b056f-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="b056f-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) активує звітування про використання та аварійне завершення роботи даних.</span><span class="sxs-lookup"><span data-stu-id="b056f-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="b056f-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) надсилає відомості про сайт, що використовується для вдосконалення служб Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b056f-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="b056f-108">Докладні відомості див. [в розділі Налаштування параметрів політики.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="b056f-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
