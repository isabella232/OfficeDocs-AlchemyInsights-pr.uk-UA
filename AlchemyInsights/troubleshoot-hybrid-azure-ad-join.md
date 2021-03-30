---
title: Виправлення неполадок із гібридним приєднанням до Microsoft Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401928"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Виправлення неполадок із гібридним приєднанням до Microsoft Azure AD

Настійно рекомендується переконатися, що пристрій має доступ до кінцевих точок служби реєстрації пристроїв під системним обліковим записом, використовуючи [сценарій перевірки підключення до служби реєстрації пристроїв](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Якщо ви вперше налаштовуєте реєстрацію пристрою, ознайомтеся зі [Вступом до керування пристроями в Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), щоб дізнатися, як установити контроль Microsoft Azure AD над пристроєм.
1. Якщо ви реєструєте пристрій безпосередньо в Microsoft Azure AD, а потім в Intune, спочатку [налаштуйте Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) і переконайтеся в наявності [ліцензій](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Переконайтеся, що ви маєте право на виконання операцій в Microsoft Azure AD та в локальній службі Active Directory. Тільки глобальний адміністратор Microsoft Azure AD може керувати параметрами реєстрації пристроїв. Крім того, щоб налаштувати автоматичну реєстрацію в локальній службі Active Directory, вам потрібно мати права адміністратора служби Active Directory та AD FS (якщо застосовується).

Додаткові відомості про усунення потенційних проблем із гібридним приєднанням див. в статті [Виправлення неполадок із гібридним приєднанням](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Щоб налаштувати гібридне приєднання до Microsoft Azure AD та керувати пристроями за допомогою порталу Microsoft Azure AD, див. статті [Налаштування пристроїв із гібридним приєднанням до Microsoft Azure AD (приєднаних до локального домену)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) та [Керування пристроями за допомогою порталу Microsoft Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Щоб усунути поширені проблеми з гібридним приєднанням до Microsoft Azure Active Directory (AD), див. статтю [Гібридне приєднання до Microsoft Azure AD: запитання й вiдповiдi](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
