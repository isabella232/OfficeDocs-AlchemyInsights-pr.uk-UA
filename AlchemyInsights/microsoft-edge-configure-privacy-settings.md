---
title: Microsoft Edge настроювання параметрів конфіденційності
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114193"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge настроювання параметрів конфіденційності

За замовчуванням, якщо Microsoft Edge розгортаються на неприборках Windows, до корпорації Майкрософт діагностичні дані та відомості про сайт не надсилаються. Однак якщо пакет Microsoft Edge на Windows 10, діагностичні дані та відомості про сайт надсилаються відповідно [до настройок діагностичних даних Windows користувачів.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Щоб налаштувати спосіб Microsoft Edge обробляє збирання даних в організації, скористайтеся наведеними нижче груповими політиками.
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)ця політика дає змогу звітувати про використання та аварійне завершення роботи даних.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ця політика надсилає відомості про сайт, які використовуються, щоб покращити служби Microsoft.

Докладні відомості див. [в розділі Налаштування параметрів політики.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)