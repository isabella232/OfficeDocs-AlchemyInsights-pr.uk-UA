---
title: Розгортання групової політики
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428048"
---
# <a name="gpo-deployment"></a>Розгортання групової політики

Настройки для об'єктів користувача та комп'ютера в службах доменів "Лазурний" (Sure AD DS) часто керуються за допомогою об'єктів групової політики (GPS). У Azure AD DS містяться вбудовані контейнери для користувачів AADDC і контейнерів для комп'ютерів AADDC. Ви можете налаштувати ці вбудовані GPOs, щоб налаштувати групову політику, як потрібно для вашого середовища. Користувачі групи «Адміністратори DC» мають права адміністрування групової політики в домені Azure AD DS, а також можуть створювати користувацькі та організаційні одиниці (OUs). Докладні відомості про групову політику та її роботу наведено в статті [Огляд групової політики](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

У гібридному середовищі групові політики, настроєні в локальній середовищі AD DS, не синхронізуються з Azure AD DS. Щоб визначити параметри конфігурації для користувачів або комп'ютерів у Azure AD DS, відредагуйте один із стандартних служб GPOs або створіть Настроюваний об'єкт групової політики.

У цій статті [керування груповою політикою](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) показано, як інсталювати засоби керування груповою політикою, як тон відредагувати вбудовану програму GTS, а також як створювати користувацькі служби gppos.
