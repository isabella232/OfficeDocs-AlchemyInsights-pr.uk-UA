---
title: Умови, відсутні в SharePoint Online термін зберігання
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053534"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="231ab-102">Увімкнення шифрування BitLocker з InTune</span><span class="sxs-lookup"><span data-stu-id="231ab-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="231ab-103">InTune endPoint Protection політики можна використовувати для настроювання Boitшафка шифрування параметри для пристроїв Windows, як описано в: Windows10 (і пізніших) параметри для захисту пристроїв за допомогою InTune</span><span class="sxs-lookup"><span data-stu-id="231ab-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="231ab-104">Слід пам'ятати, що багато нових пристроїв під керуванням Windows 10 підтримують автоматичне шифрування BitLocker, який запускається без застосування політики MDM.</span><span class="sxs-lookup"><span data-stu-id="231ab-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="231ab-105">Це може вплинути на застосування політики, якщо не настроєно параметри за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="231ab-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="231ab-106">Дивіться FAQ для більш детального перегляду.</span><span class="sxs-lookup"><span data-stu-id="231ab-106">See FAQ for more detail.</span></span>


<span data-ttu-id="231ab-107">FAQ  Q: які випуски Windows підтримують шифрування пристрою за допомогою кінцевої точки захисту політики?</span><span class="sxs-lookup"><span data-stu-id="231ab-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="231ab-108"> В: параметри, в InTune endPoint Protection політики здійснюється за допомогою засобу BitLocker.</span><span class="sxs-lookup"><span data-stu-id="231ab-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="231ab-109">Не всі випуски та збірки Windows підтримують засіб BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="231ab-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="231ab-110">У цей час випуски Windows: підприємство; Підтримуються освітні, мобільні, мобільні підприємства та професійні (від будівництва 1809 р.).</span><span class="sxs-lookup"><span data-stu-id="231ab-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="231ab-111">П: Якщо пристрій вже зашифровано за допомогою засобу BitLocker з використанням параметрів ОС за замовчуванням для методу шифрування та міцності шифру (XTS-AES-128) буде застосовувати політику з різними налаштуваннями автоматично ініціювати повторне шифрування диска з новими налаштуваннями?</span><span class="sxs-lookup"><span data-stu-id="231ab-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="231ab-112">A: ні.</span><span class="sxs-lookup"><span data-stu-id="231ab-112">A: No.</span></span> <span data-ttu-id="231ab-113">Для того, щоб застосувати нові параметри шифру, диск спочатку потрібно розшифрувати.</span><span class="sxs-lookup"><span data-stu-id="231ab-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="231ab-114">Примітка для пристроїв, що навчаються з Автопілот автоматичне шифрування, яке буде відбуватися під час першого запуску не запускається, доки політики InTune оцінюється, який дозволяє політики на основі параметрів для використання на місці ОС за промовчанням</span><span class="sxs-lookup"><span data-stu-id="231ab-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="231ab-115">П Якщо пристрій зашифровано в результаті застосування політики InTune буде розшифровано під час видалення цієї політики?</span><span class="sxs-lookup"><span data-stu-id="231ab-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="231ab-116">A: видалення, пов'язані з шифрування політики не призводить до дешифрування дисків, які настроєно.</span><span class="sxs-lookup"><span data-stu-id="231ab-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="231ab-117">П: чому політики щодо дотримання InTune показують, що мій пристрій не має "BitLocker включений", але це?</span><span class="sxs-lookup"><span data-stu-id="231ab-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="231ab-118">В: параметр "BitLocker з підтримкою" у InTune політики дотримання використовує клієнт Windows пристрій атестації здоров'я (ДГВ).</span><span class="sxs-lookup"><span data-stu-id="231ab-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="231ab-119">Цей клієнт лише вимірює стан пристрою під час завантаження.</span><span class="sxs-lookup"><span data-stu-id="231ab-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="231ab-120">Таким чином, якщо пристрій не було перезавантажено після того, як шифрування BitLocker було завершено, служба для клієнтів ДГВ не повідомляє засобу BitLocker як активний.</span><span class="sxs-lookup"><span data-stu-id="231ab-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>