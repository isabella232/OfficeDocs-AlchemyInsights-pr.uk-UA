---
title: Ключі відновлення Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505089"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Доступ до ключів відновлення Bitlocker

Налаштовування політики захисту кінцевої точки Intune із Bitlocker можна визначити, чи слід зберігати відомості про відновлення Bitlocker в Azure Active Directory.

Якщо цей параметр налаштовано, збережені дані відновлення мають бути видимі для адміністратора Intune як частина даних запису пристрою в Intune Devices blade двома способами:

Пристрої – пристрої з Azure AD > "Пристрій" або "Пристрої> "Усі пристрої" –> "Пристрій" –> відновлення

Крім того, якщо є адміністративний доступ до пристрою, ключ відновлення (Пароль) можна переглянути, виконавши таку команду в командному рядку в режимі адміністратора:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Якщо пристрій зашифровано до реєстрації в Intune, ключ відновлення, можливо, пов'язано з "Обліковим записом Microsoft" (MSA), який використовувався для входу на пристрій під час процесу УБЗ. У такому разі для доступу до служби MSA і входу в неї мають відображатися пристрої, для яких  https://onedrive.live.com/recoverykey збережено ключі відновлення.
 
Якщо пристрій зашифровано через групову політику на основі домену, відомості про відновлення можуть зберігатися в локальній службі Active Directory.

Якщо ви налаштували політику захисту кінцевих точок на зберігання ключа відновлення в Azure Active Directory, але ключ для певного пристрою не передано, ви можете ініціювати передавання, поворотивши ключ відновлення цього пристрою з консолі mem. Докладні відомості див. [в розділах Повертання ключів відновлення BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

