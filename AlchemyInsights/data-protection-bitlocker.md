---
title: Захист даних — засіб BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908730"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="532ec-102">Увімкнення шифрування BitLocker з InTune</span><span class="sxs-lookup"><span data-stu-id="532ec-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="532ec-103">InTune endPoint Protection політики можна використовувати для настроювання параметрів шифрування BitLocker для пристроїв Windows.</span><span class="sxs-lookup"><span data-stu-id="532ec-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="532ec-104">Додаткові відомості наведено в розділі [Параметри Windows 10 (і пізніших версій) для захисту пристроїв за допомогою InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="532ec-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="532ec-105">Слід пам'ятати, що багато нових пристроїв під керуванням Windows 10 підтримують автоматичне шифрування BitLocker, яке запускається без застосування політики MDM.</span><span class="sxs-lookup"><span data-stu-id="532ec-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="532ec-106">Це може вплинути на застосування політики, якщо налаштовані не за промовчанням параметри.</span><span class="sxs-lookup"><span data-stu-id="532ec-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="532ec-107">Докладніші відомості наведено в таких ВІДПОВІДЯХ.</span><span class="sxs-lookup"><span data-stu-id="532ec-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="532ec-108">Щоб отримати відомості про виправлення неполадок, пов'язаних із BitLocker, див. [виправлення політики BitLocker, у Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="532ec-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="532ec-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="532ec-109">**FAQ**</span></span>

 <span data-ttu-id="532ec-110">П: які випуски шифрування пристрою підтримують Windows за допомогою політики кінцевої точки захисту?</span><span class="sxs-lookup"><span data-stu-id="532ec-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="532ec-111">В: параметри, в InTune endPoint Protection політики здійснюється за допомогою засобу [BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="532ec-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="532ec-112">Не всі випуски або збірки Windows підтримують засіб BitLocker.</span><span class="sxs-lookup"><span data-stu-id="532ec-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="532ec-113">На даний момент підтримуються наступні випуски Windows: підприємство, освіта, мобільний, мобільний підприємство, і професійний (Build 1809 і пізніших версій).</span><span class="sxs-lookup"><span data-stu-id="532ec-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="532ec-114">П: Якщо пристрій вже зашифровано за допомогою засобу BitLocker, використовуючи настройки ОС за замовчуванням для методу шифрування та міцності шифру (XTS-AES-128), буде застосовуватися політика з різними налаштуваннями автоматично ініціювати повторне шифрування диска з новими налаштуваннями?</span><span class="sxs-lookup"><span data-stu-id="532ec-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="532ec-115">A: ні.</span><span class="sxs-lookup"><span data-stu-id="532ec-115">A: No.</span></span> <span data-ttu-id="532ec-116">Щоб застосувати нові параметри шифру, диск спочатку потрібно розшифрувати.</span><span class="sxs-lookup"><span data-stu-id="532ec-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="532ec-117">**Примітка:** Для пристроїв, що навчаються за допомогою автопілота, автоматичне шифрування, яке буде відбуватися під час першого запуску не запускається до того, як InTune політики буде оцінено, що дозволяє параметри на основі політики, які використовуватимуться замість ОС за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="532ec-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="532ec-118">П: Якщо пристрій зашифровано в результаті застосування політики InTune, його буде розшифровано під час видалення цієї політики?</span><span class="sxs-lookup"><span data-stu-id="532ec-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="532ec-119">A: видалення, пов'язані з шифрування політики не призводить до дешифрування дисків, які настроєно.</span><span class="sxs-lookup"><span data-stu-id="532ec-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="532ec-120">П: чому політика щодо дотримання InTune показує, що пристрій не підтримує BitLocker, хоча це?</span><span class="sxs-lookup"><span data-stu-id="532ec-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="532ec-121">В: параметр "BitLocker з підтримкою" у політиці дотримання InTune використовує клієнта Windows пристрій атестації здоров'я (ДГВ).</span><span class="sxs-lookup"><span data-stu-id="532ec-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="532ec-122">Цей клієнт лише вимірює стан пристрою під час завантаження.</span><span class="sxs-lookup"><span data-stu-id="532ec-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="532ec-123">Тому, якщо пристрій не було перезавантажено після завершення шифрування BitLocker, служба клієнта ДГВ не повідомить про засіб BitLocker як активний.</span><span class="sxs-lookup"><span data-stu-id="532ec-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 