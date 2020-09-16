---
title: DataProtection – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731260"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="64ae7-102">Увімкнення шифрування BitLocker за допомогою функції Inune</span><span class="sxs-lookup"><span data-stu-id="64ae7-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="64ae7-103">Можна використовувати політику захисту від кінцевої точки, щоб настроїти параметри шифрування BitLocker для пристроїв із Windows.</span><span class="sxs-lookup"><span data-stu-id="64ae7-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="64ae7-104">Щоб отримати докладніші відомості, ознайомтеся [з настройками Windows 10 (і новіших версій), щоб захистити пристрої за допомогою функції Inune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="64ae7-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="64ae7-105">Ви маєте знати, що багато нових пристроїв під керуванням Windows 10 підтримують автоматичне шифрування BitLocker, яке спрацьовує без використання політики MDM.</span><span class="sxs-lookup"><span data-stu-id="64ae7-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="64ae7-106">Це може вплинути на застосування політики, якщо настроєно параметри, які не використовуються за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="64ae7-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="64ae7-107">Перегляньте наведені нижче запитання й відповіді про докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="64ae7-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="64ae7-108">Докладні відомості про виправлення неполадок програми BitLocker наведено [в статті виправлення неполадок політики BitLocker в Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="64ae7-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="64ae7-109">**Запитання й відповіді**</span><span class="sxs-lookup"><span data-stu-id="64ae7-109">**FAQ**</span></span>

 <span data-ttu-id="64ae7-110">Запитання: які випуски шифрування пристроїв підтримки Windows використовують політику захисту від кінцевої точки?</span><span class="sxs-lookup"><span data-stu-id="64ae7-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="64ae7-111">В: параметри політики захисту кінцевої точки Inune реалізуються в програмі [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="64ae7-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="64ae7-112">Не всі випуски або збірки Windows підтримують програму BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="64ae7-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="64ae7-113">Цього разу підтримуються такі випуски Windows: Enterprise, Education, Mobile, Mobile Enterprise і Professional (збірка 1809 і пізніші).</span><span class="sxs-lookup"><span data-stu-id="64ae7-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="64ae7-114">П: Якщо пристрій уже зашифровано за допомогою засобу BitLocker, використовуючи настройки за замовчуванням ОС для методу шифрування та міцність шифру (XTS-AES-128), буде застосовуватися політика з різними настройками, щоб автоматично ініціювати повторне шифрування диска з новими настройками?</span><span class="sxs-lookup"><span data-stu-id="64ae7-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="64ae7-115">Відповідь. Ні.</span><span class="sxs-lookup"><span data-stu-id="64ae7-115">A: No.</span></span> <span data-ttu-id="64ae7-116">Щоб додати нові параметри шифру, диск спочатку має бути розшифровано.</span><span class="sxs-lookup"><span data-stu-id="64ae7-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="64ae7-117">**Примітка.** Для пристроїв, які ви зареєстровані в автопілоті, автоматичне шифрування, яке відбуватиметься під час першого запуску, не спрацьовує, доки не буде обчислено політику Inune, яка дає змогу використовувати параметри, які використовуються на основі стандартних параметрів операційної системи.</span><span class="sxs-lookup"><span data-stu-id="64ae7-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="64ae7-118">П: Якщо пристрій зашифровано в результаті застосування політики Inune, його буде розшифровано після видалення цієї політики?</span><span class="sxs-lookup"><span data-stu-id="64ae7-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="64ae7-119">В: видалення політики, пов'язаної з шифруванням, не призводить до розшифрування дисків, які було настроєно.</span><span class="sxs-lookup"><span data-stu-id="64ae7-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="64ae7-120">Питання: Чому в політиці відповідності не активовано функцію BitLocker, хоча в моєму пристрої немає увімкнутих пристроїв.</span><span class="sxs-lookup"><span data-stu-id="64ae7-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="64ae7-121">В: у політиці відповідності "Увімкнення BitLocker" використовується клієнт атестації для пристроїв Windows (ДГВ).</span><span class="sxs-lookup"><span data-stu-id="64ae7-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="64ae7-122">Цей клієнт лише вимірює стан пристрою під час завантаження.</span><span class="sxs-lookup"><span data-stu-id="64ae7-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="64ae7-123">Тому, якщо пристрій не перезавантажиться після завершення шифрування BitLocker, клієнтську службу DHA не повідомляють про те, що програма BitLocker буде активна.</span><span class="sxs-lookup"><span data-stu-id="64ae7-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 