---
title: Розгортання GPO
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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067861"
---
# <a name="gpo-deployment"></a>Розгортання GPO

Настройки об'єктами користувачів і комп'ютерів у службах доменів Azure Active Directory (Azure AD DS) часто керуються за допомогою об'єктів групової політики. Служба Azure AD DS включає вбудовані об'ємні об'єми для користувачів AADDC і контейнерів AADDC Computers. Ці вбудовані об'єктні об'єкти (GPOS) можна налаштувати так, щоб вони налаштовувалися за потреби для свого середовища. Учасники групи адміністраторів Azure AD DC мають права адміністратора групової політики в домені Azure AD DS, а також можуть створювати настроювані об'єкти групової політики та організаційні одиниці. Докладні відомості про групову політику та її принцип роботи див. в статті Огляд [групової політики.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

У гібридному середовищі групові політики, налаштовані в локальному середовищі AD DS, не синхронізуються з Azure AD DS. Щоб визначити параметри конфігурації для користувачів або комп'ютерів в Azure AD DS, відредагувати один зі стандартних GPO або створити настроюваний об'пункт групової політики.

У цій статті [описано,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) як інсталювати інструменти керування груповою політикою, змінити вбудований об'єкт групової політики та створити власні об'єктної політики.
