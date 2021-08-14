---
title: Дозволи та згода API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932118"
---
# <a name="api-permissions-and-consent"></a>Дозволи API та згода

Програми, які інтегруються платформа ідентичностей Microsoft до моделі авторизації, яка надає користувачам і адміністраторам контроль над доступом до даних. Впровадження моделі авторизації оновлено на кінцевій платформа ідентичностей Microsoft кінцевій точці. У ньому змінюється спосіб взаємодії програми з платформа ідентичностей Microsoft. [Дозволи та згода](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) в платформа ідентичностей Microsoft кінцевій точці охоплює основні поняття цієї моделі авторизації, зокрема області, дозволи та згоду.

Структура [згоди Azure Active Directory клієнта (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) дає змогу розробляти веб-програми для кількох клієнтів і власні клієнтські програми. Ці програми дають змогу входити за допомогою облікових записів користувачів із клієнта Azure AD, відмінного від того, у якому зареєстровано програму. Крім Graph інтерфейсів API веб-інтерфейсів (для доступу до Azure AD, Intune і служб в Microsoft 365) та інших інтерфейсів API веб-інтерфейсів (API) служби Microsoft, їм, можливо, знадобиться отримати доступ до інтерфейсів API веб-інтерфейсів (Azure AD, Intune) та інших інтерфейсів API служби Microsoft.

