---
title: Настроювання LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885582"
---
# <a name="configure-ldap"></a>Настроювання LDAP

Щоб настроїти LDAP, виконайте наведені нижче дії.

1. Перевірте стан справності свого домену на [порталі Azure](https://aka.ms/aadds-health).
1. Переконайтеся, що доступна дійсна Передплата Azure AD, і служби "Лазурний домен AD" активовано.
1. Сертифікат, який потрібно ввімкнути для захищеного LDAP, має бути отримано з надійного центру сертифікації або бути сертифікатом, що самостійно підписано.
1. Переконайтеся, що сертифікат слід відповідно до потрібних [рекомендацій](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Неприпустимий сертифікат**
1. Щоб поновити сертифікат, дотримуйтеся вказівок, щоб створити новий сертифікат і повторно передати його: [НАСТРОЮВАННЯ LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Щоб вирішити відому проблему з Захищенними оповіщеннями LDAP у службах домену Azure Active Directory, ознайомтеся з [вирішенням СПОВІЩЕНЬ LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
