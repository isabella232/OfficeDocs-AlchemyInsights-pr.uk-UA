---
title: Privileged Identity Management ролі
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973250"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management (PIM)

**Дозволи не надаються після активації ролі**

Активація ролі в Azure AD Privileged Identity Management (PIM) може миттєво починатись не на всі портали, для яких потрібна привілейована роль. Іноді навіть якщо зміна почнеться, кешування в Інтернеті на порталі може призвести до того, що зміна не набирає сили відразу.

Якщо активація затримується, виконайте такі дії:

1. Вийдіть із порталу Azure, а потім увійдіть знову. Коли ви активуєте роль Azure AD або роль ресурсу Azure, ви побачите етапи активації. Коли всі етапи завершаться, з'явиться посилання "Вийти". За цим посиланням можна вийти. У більшості випадків це вирішує проблему із затримкою активації.
2. У PIM переконайтеся, що вас зазначено як учасника ролі.
3. Якщо ви активували роль адміністратора Exchange, обов'язково вийдіть і ввійдіть знову. Якщо проблема не зникне, відкрийте запит на підтримку та підніміть його як проблему. Якщо для доступу до Центру безпеки та відповідності використовується роль Exchange, див. наступний крок.
4. Під час активації ролі для доступу до Центру безпеки та відповідності або для активації ролі адміністратора SharePoint активації може виникнути певна затримка активації від кількох хвилин до кількох годин. Це відома проблема, і ми активно працюємо з цими командами, щоб якомога швидше вирішити цю проблему.

Докладні відомості:

- [Активація ролей Azure AD у PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Активація ролей ресурсів Azure у PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Дозволи не видаляються після деактивації ролі або завершення терміну дії активації ролей**

Якщо деактивувати роль в Azure AD Privileged Identity Management період активації ролей, може статися затримка, через яку ви й надалі матимете доступ.

Якщо деактивація затримується, виконайте такі дії:

1. Якщо ви деактивували роль адміністратора Exchange або завершиться термін дії періоду активації ролей і ви помітили значну затримку, перш ніж видаляти дозволи, відкрийте запит на підтримку та повідомте інженера служби підтримки, щоб допомогти вам покласти запит до команди керування привілейованим доступом (PAM) Office про цю проблему.
2. Якщо термін дії періоду активації минув, але сеанс браузера все одно відкрито, закрийте браузер. Ви можете використовувати цю роль, доки не закриєте цей сеанс. Це відома проблема, і ми розглянемо потенційне виправлення, яке полягає в тому, щоб активно відкликати кожен сеанс після завершення активації.

Якщо затримка відрізняється від цих двох сценаріїв, відкрийте запит на підтримку.
