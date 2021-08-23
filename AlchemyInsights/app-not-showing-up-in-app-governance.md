---
title: Моя програма не відображається в регуляторі програм
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454986"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Моя програма не відображається в регуляторі програм

Якщо ваша програма не відображається в регуляторі програми, перевірте таке:

1. Перейдіть до [служби Azure AD](https://aad.portal.azure.com/) та знайдіть ідентифікатор програми, шукаючи її ім'я у верхньому рядку на сторінці "Огляд".

1. Access Graph Explorer і знайдіть ідентифікатор програми в основному вікні служби, використовуючи цей запит і замінивши відповідний ідентифікатор <appId> програми: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Якщо результатів не знайдено, знайдіть ідентифікатор програми в програмі за допомогою цього запиту та замініть його на відповідний ідентифікатор <appId> програми: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Якщо у вас виникають проблеми із запитом, див. [отримайте підтримку.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Докладні відомості або ілюстрування програм, що вводяться в програмі, див. в цій [службі.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Докладні відомості про перегляд програм див. в [статті Перегляд програм.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
