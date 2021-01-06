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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768838"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="0255c-102">Увімкнення шифрування BitLocker за допомогою функції Inune</span><span class="sxs-lookup"><span data-stu-id="0255c-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="0255c-103">Можна використовувати політику захисту від кінцевої точки, щоб настроїти параметри шифрування BitLocker для пристроїв із Windows.</span><span class="sxs-lookup"><span data-stu-id="0255c-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="0255c-104">Щоб отримати докладніші відомості, ознайомтеся [з настройками Windows 10 (і новіших версій), щоб захистити пристрої за допомогою функції Inune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="0255c-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="0255c-105">Ви маєте знати, що багато нових пристроїв під керуванням Windows 10 підтримують автоматичне шифрування BitLocker, яке спрацьовує без використання політики MDM.</span><span class="sxs-lookup"><span data-stu-id="0255c-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="0255c-106">Це може вплинути на застосування політики, якщо настроєно параметри, які не використовуються за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="0255c-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="0255c-107">Перегляньте наведені нижче запитання й відповіді про докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="0255c-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="0255c-108">Докладні відомості про виправлення неполадок програми BitLocker наведено [в статті виправлення неполадок політики BitLocker в Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="0255c-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="0255c-109">**Запитання й відповіді**</span><span class="sxs-lookup"><span data-stu-id="0255c-109">**FAQ**</span></span>

<span data-ttu-id="0255c-110">Запитання: які випуски шифрування пристроїв підтримки Windows використовують політику захисту від кінцевої точки?</span><span class="sxs-lookup"><span data-stu-id="0255c-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="0255c-111">В: параметри політики захисту кінцевої точки Inune реалізуються в програмі [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="0255c-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="0255c-112">Не всі випуски або збірки Windows підтримують програму BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="0255c-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="0255c-113">Запитання: як можна ввімкнути функцію BitLocker на пристроях, не вимагаючи взаємодії з кінцевим користувачем?</span><span class="sxs-lookup"><span data-stu-id="0255c-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="0255c-114">Відповіді: доки необхідні обов'язкові передумови, можна ввімкнути засіб BitLocker "мовчазний шифрування" на веб-сторінці Inune.</span><span class="sxs-lookup"><span data-stu-id="0255c-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="0255c-115">Перегляньте відомості про вимоги до пристрою та параметри політики прикладу, щоб увімкнути безшумний шифрування в цьому документі: [мовчки Увімкніть шифрування BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="0255c-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="0255c-116">П: Якщо пристрій уже зашифровано за допомогою засобу BitLocker, використовуючи настройки за замовчуванням ОС для методу шифрування та міцність шифру (XTS-AES-128), буде застосовуватися політика з різними настройками, щоб автоматично ініціювати повторне шифрування диска з новими настройками?</span><span class="sxs-lookup"><span data-stu-id="0255c-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="0255c-117">Відповідь. Ні.</span><span class="sxs-lookup"><span data-stu-id="0255c-117">A: No.</span></span> <span data-ttu-id="0255c-118">Щоб додати нові параметри шифру, диск спочатку має бути розшифровано.</span><span class="sxs-lookup"><span data-stu-id="0255c-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="0255c-119">**Примітка.** Для пристроїв, які ви зареєстровані в автопілоті, автоматичне шифрування, яке відбуватиметься під час першого запуску, не спрацьовує, доки не буде обчислено політику Inune, яка дає змогу використовувати параметри, які використовуються на основі стандартних параметрів операційної системи.</span><span class="sxs-lookup"><span data-stu-id="0255c-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="0255c-120">П: Якщо пристрій зашифровано в результаті застосування політики Inune, його буде розшифровано після видалення цієї політики?</span><span class="sxs-lookup"><span data-stu-id="0255c-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="0255c-121">В: видалення політики, пов'язаної з шифруванням, не призводить до розшифрування дисків, які було настроєно.</span><span class="sxs-lookup"><span data-stu-id="0255c-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="0255c-122">Питання: Чому в політиці відповідності не активовано функцію BitLocker, хоча в моєму пристрої немає увімкнутих пристроїв.</span><span class="sxs-lookup"><span data-stu-id="0255c-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="0255c-123">В: у політиці відповідності "Увімкнення BitLocker" використовується клієнт атестації для пристроїв Windows (ДГВ).</span><span class="sxs-lookup"><span data-stu-id="0255c-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="0255c-124">Цей клієнт лише вимірює стан пристрою під час завантаження.</span><span class="sxs-lookup"><span data-stu-id="0255c-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="0255c-125">Тому, якщо пристрій не перезавантажиться після завершення шифрування BitLocker, клієнтську службу DHA не повідомляють про те, що програма BitLocker буде активна.</span><span class="sxs-lookup"><span data-stu-id="0255c-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 