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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090433"
---
# <a name="configure-ldap"></a>Настроювання LDAP

Щоб настроїти LDAP, виконайте такі дії:

1. Перевірте справність свого домену на [порталі Azure.](https://aka.ms/aadds-health)
1. Переконайтеся, що доступна дійсна передплата на Azure AD, а служби доменів Azure AD активовано.
1. Сертифікат, необхідний для ввімкнення захищеного протоколу LDAP, потрібно отримати в надійного загальнодоступного центру сертифікації або сертифікат із власним підписом.
1. Переконайтеся, що сертифікат має дотримуватися [обов'язкових рекомендацій](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Недійсний сертифікат**
1. Щоб поновити сертифікат, виконайте кроки, щоб створити новий сертифікат і перезавантажити його: [Настроювання LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Відомості про вирішення відомої проблеми з оповіщеннями Secure LDAP у службі доменів Azure Active Directory див. в розділі Вирішення оповіщень [LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
