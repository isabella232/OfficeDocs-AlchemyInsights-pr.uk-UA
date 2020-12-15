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
# <a name="microsoft-edge-configure-privacy-settings"></a>Настроювання параметрів конфіденційності Microsoft EDGE

За замовчуванням, якщо Microsoft EDGE розгорнуто на платформах, які не є ОС Windows, діагностичні дані та відомості про сайт не надсилатимуться до корпорації Майкрософт. Однак, якщо Microsoft EDGE розгорнуто в ОС Windows 10, діагностичні дані та відомості про сайт надсилатиметься відповідно до [параметрів діагностики даних Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Ось як настроїти колекцію даних Microsoft EDGE для організації, використовуючи наведені нижче групові політики.
- Параметри [метаданих](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ця політика дає змогу повідомляти про використання та дані, пов'язані з аварійними даними.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ця політика надсилає відомості про сайт, які використовуються для вдосконалення служб Microsoft.

Докладні відомості наведено в статті [Настроювання параметрів політики](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).