---
title: Групова політика
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256910"
---
# <a name="group-policy"></a>Групова політика

Настройки для об'єктів користувача та комп'ютера в службах доменів "Лазурний" (Sure AD DS) часто керуються за допомогою об'єктів групової політики (GPS). У Azure AD DS містяться вбудовані контейнери для користувачів AADDC і контейнерів для комп'ютерів AADDC. Ви можете налаштувати ці вбудовані GPOs, щоб налаштувати групову політику, як потрібно для вашого середовища. Користувачі групи «Адміністратори DC» мають права адміністрування групової політики в домені Azure AD DS, а також можуть створювати користувацькі та організаційні одиниці (OUs). Докладні відомості про групову політику та її роботу наведено в статті [Огляд групової політики](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

У гібридному середовищі групові політики, настроєні в локальній середовищі AD DS, не синхронізуються з Azure AD DS. Щоб визначити параметри конфігурації для користувачів або комп'ютерів у Azure AD DS, відредагуйте один із стандартних служб GPOs або створіть Настроюваний об'єкт групової політики.

У цій статті [керування груповою політикою](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) показано, як інсталювати засоби керування груповою політикою, як тон відредагувати вбудовану програму GTS, а також як створювати користувацькі служби gppos.



