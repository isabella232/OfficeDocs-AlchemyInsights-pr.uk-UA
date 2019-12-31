---
title: Ключі відновлення BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908835"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Доступ до ключів відновлення BitLocker

Під час настроювання параметрів BitLocker, InTune endPoint Protection політики, можна визначити, чи слід зберігати відомості відновлення BitLocker в Azure Active Directory.

Якщо цей параметр налаштовано, дані для відновлення зберігаються на InTune адміністратора як частину даних запису пристрою в InTune пристроїв Blade двома способами:

Пристрої-Azure AD-пристрої > "пристрій" або пристрої-> всі пристрої-> "пристрій"-> відновлення ключів

Крім того, якщо є адміністративний доступ до самого пристрою, ключ відновлення (пароль) можна побачити, виконавши таку команду в командному рядку в режимі адміністратора:

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
Якщо пристрій було зашифровано до зарахування в InTune, ключ відновлення може бути пов'язано з "обліковий запис Microsoft" (MSA), який використовується для входу на пристрій під час першого запуску. Якщо це так, доступ https://onedrive.live.com/recoverykey і вхід в с, що MSA повинні показати пристрої, для яких були збережені ключі відновлення.
 
Якщо пристрій було зашифровано в результаті конфігурації за допомогою доменної групової політики, відомості про відновлення можуть зберігатися в локально Active Directory.
 

