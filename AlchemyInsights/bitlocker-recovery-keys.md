---
title: Ключі відновлення Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820307"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="b35fa-102">Доступ до ключів відновлення Bitlocker</span><span class="sxs-lookup"><span data-stu-id="b35fa-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="b35fa-103">Налаштовування політики захисту кінцевої точки Intune із Bitlocker можна визначити, чи слід зберігати відомості про відновлення Bitlocker в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b35fa-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="b35fa-104">Якщо цей параметр налаштовано, збережені дані відновлення мають бути видимі для адміністратора Intune як частина даних запису пристрою в Intune Devices blade двома способами:</span><span class="sxs-lookup"><span data-stu-id="b35fa-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="b35fa-105">Пристрої – пристрої з Azure AD > "Пристрій" або "Пристрої> "Усі пристрої" –> "Пристрій" –> відновлення</span><span class="sxs-lookup"><span data-stu-id="b35fa-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="b35fa-106">Крім того, якщо є адміністративний доступ до пристрою, ключ відновлення (Пароль) можна переглянути, виконавши таку команду в командному рядку в режимі адміністратора:</span><span class="sxs-lookup"><span data-stu-id="b35fa-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="b35fa-107">Якщо пристрій зашифровано до реєстрації в Intune, ключ відновлення, можливо, пов'язано з "Обліковим записом Microsoft" (MSA), який використовувався для входу на пристрій під час процесу УБЗ.</span><span class="sxs-lookup"><span data-stu-id="b35fa-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="b35fa-108">У такому разі для доступу до служби MSA і входу в неї мають відображатися пристрої, для яких  https://onedrive.live.com/recoverykey збережено ключі відновлення.</span><span class="sxs-lookup"><span data-stu-id="b35fa-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="b35fa-109">Якщо пристрій зашифровано через групову політику на основі домену, відомості про відновлення можуть зберігатися в локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b35fa-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="b35fa-110">Якщо ви налаштували політику захисту кінцевих точок на зберігання ключа відновлення в Azure Active Directory, але ключ для певного пристрою не передано, ви можете ініціювати передавання, поворотивши ключ відновлення цього пристрою з консолі mem.</span><span class="sxs-lookup"><span data-stu-id="b35fa-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="b35fa-111">Докладні відомості див. [в розділах Повертання ключів відновлення BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="b35fa-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

