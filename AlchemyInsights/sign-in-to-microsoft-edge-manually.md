---
title: Вхід у Microsoft Edge вручну
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398678"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Вхід у Microsoft Edge вручну

Якщо користувач не входив автоматично під час першого запуску, користувач може вручну ввійти в настройки браузера або вилітає ідентичність. Щоб керувати входом, використовуйте такі політики:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – щоб користувач завжди був із робочим профілем у Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – обмеження входу до набору надійних облікових записів.
3. [BrowserSignin –](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) вимкнення входу або примусове входу користувачів.

