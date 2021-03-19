---
title: Ключі відновлення BitLocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685907"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="d3fdd-102">Доступ до ключів відновлення BitLocker</span><span class="sxs-lookup"><span data-stu-id="d3fdd-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="d3fdd-103">Під час настроювання політики захисту кінцевої точки в службі BitLocker можна визначити, чи потрібно зберегти відомості про відновлення засобу BitLocker в "лазуровому Active Directory".</span><span class="sxs-lookup"><span data-stu-id="d3fdd-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="d3fdd-104">Якщо цей параметр настроєно, дані, які зберігається, повинні бути видимі для адміністратора Inune, що входить до складу даних запису пристрою на пристроях Inune, двома способами:</span><span class="sxs-lookup"><span data-stu-id="d3fdd-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="d3fdd-105">Пристрої-блакитні РЕКЛАМНІ пристрої-> "пристрій" або пристрої-> всі пристрої-> "пристрій"-> ключів відновлення</span><span class="sxs-lookup"><span data-stu-id="d3fdd-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="d3fdd-106">Крім того, якщо для самого пристрою є адміністративний доступ, ключ відновлення (пароль) можна побачити, виконавши таку команду з командного рядка підвищеної якості:</span><span class="sxs-lookup"><span data-stu-id="d3fdd-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="d3fdd-107">Якщо пристрій було зашифровано перед зарахацією в Inune, ключ відновлення може бути пов'язано з "обліковим записом Microsoft" (MSA), що використовується для входу на пристрій під час першого запуску.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="d3fdd-108">Якщо це було так, доступ  https://onedrive.live.com/recoverykey і вхід за допомогою цієї функції MSA має відображати пристрої, для яких були збережені ключі відновлення.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="d3fdd-109">Якщо пристрій зашифровано як результат конфігурації за допомогою групової політики на основі доменів, відомості про відновлення можуть зберігатися в локальному Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

