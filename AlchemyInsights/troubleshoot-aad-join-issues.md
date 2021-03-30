---
title: Усунення несправностей, пов'язаних із приєднанням до Azure
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405765"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Усунення несправностей, пов'язаних із приєднанням до Azure

1. Якщо ви вперше настроєте реєстрацію пристроїв, перевірте загальні відомості про керування пристроями в [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) що допоможе вам отримати пристрої під контролем в Azure AD. 
1. Якщо ви реєструєте пристрої безпосередньо в Azure AD та зареєстрували їх в Intune, переконайтеся, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) що ви налаштували [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) і ліцензування настроїли спочатку.
1. Переконайтеся, що ви маєте право виконувати операції в Azure AD. Лише глобальний адміністратор в Azure AD може керувати параметрами реєстрації пристроїв.
1. Відомості про те, як виконати приєднання до Azure AD, див. в [статтях Планування Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Докладні відомості про вирішення поширених проблем із приєднанням до Azure AD див. в статтях [Azure Ad Join:](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) запитання й відповіді та пристрій для Windows 10 pro див. в статті Не вдається приєднатися до комп'ютера з [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) до Azure AD – Потрібно оновити до – Спільнота Microsoft
