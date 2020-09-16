---
title: Умови відсутності з магазину термінів служби SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750472"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="79525-102">Увімкнення шифрування BitLocker за допомогою функції Inune</span><span class="sxs-lookup"><span data-stu-id="79525-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="79525-103">Політика захисту від кінцевих точок, що використовується для налаштування шифрування Boitlocker для пристроїв із Windows, як описано в таких параметрах: Windows10 (і новіші), щоб захистити пристрої за допомогою Inteune</span><span class="sxs-lookup"><span data-stu-id="79525-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="79525-104">Ви маєте знати, що багато нових пристроїв під керуванням Windows 10 підтримують автоматичне шифрування BitLocker, яке спрацьовує без використання політики MDM.</span><span class="sxs-lookup"><span data-stu-id="79525-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="79525-105">Це може вплинути на застосування політики, якщо настройки за замовчуванням не настроєно.</span><span class="sxs-lookup"><span data-stu-id="79525-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="79525-106">Докладні відомості наведено в статті запитання й відповіді.</span><span class="sxs-lookup"><span data-stu-id="79525-106">See FAQ for more detail.</span></span>


<span data-ttu-id="79525-107">Запитання й відповіді   : які випуски шифрування пристроїв підтримки Windows за допомогою політики захисту від кінцевої точки?</span><span class="sxs-lookup"><span data-stu-id="79525-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="79525-108"> В: параметри політики захисту кінцевої точки Inune реалізуються в програмі BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="79525-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="79525-109">Не всі випуски, а також збірки Windows підтримують програму BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="79525-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="79525-110">На цей раз у випусках Windows: Enterprise; Підтримуються навчальні, мобільні та мобільні підприємства (зі збірки 1809 р.).</span><span class="sxs-lookup"><span data-stu-id="79525-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="79525-111">П: Якщо пристрій уже зашифровано за допомогою засобу BitLocker, використовуючи настройки за замовчуванням ОС для методу шифрування та міцність шифру (XTS-AES-128), буде застосовуватися політика з різними настройками, щоб автоматично ініціювати повторне шифрування диска з новими настройками?</span><span class="sxs-lookup"><span data-stu-id="79525-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="79525-112">Відповідь. Ні.</span><span class="sxs-lookup"><span data-stu-id="79525-112">A: No.</span></span> <span data-ttu-id="79525-113">Щоб додати нові параметри шифру, спочатку потрібно розшифрувати диск.</span><span class="sxs-lookup"><span data-stu-id="79525-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="79525-114">Примітка для пристроїв, що підлягають реєстрації в автопілоті автоматичне шифрування, яке відбуватиметься під час першого запуску, не спрацьовує, доки не буде обчислено політику, яка дає змогу використовувати параметри політики на місці за замовчуванням для ОС.</span><span class="sxs-lookup"><span data-stu-id="79525-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="79525-115">У випадку, якщо пристрій зашифровано в результаті використання політики Inune, його буде розшифровано, коли цю політику буде видалено?</span><span class="sxs-lookup"><span data-stu-id="79525-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="79525-116">В: видалення пов'язаної політики шифрування не призводить до розшифрування дисків, які було настроєно.</span><span class="sxs-lookup"><span data-stu-id="79525-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="79525-117">Питання: Чому в політиці відповідності, що не містить "BitLocker увімкнуто"?</span><span class="sxs-lookup"><span data-stu-id="79525-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="79525-118">В: у політиці відповідності "BitLocker увімкнуто" використовується клієнт атестації для пристроїв Windows (ДГВ).</span><span class="sxs-lookup"><span data-stu-id="79525-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="79525-119">Цей клієнт лише вимірює стан пристрою під час завантаження.</span><span class="sxs-lookup"><span data-stu-id="79525-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="79525-120">Тому, якщо пристрій не перезавантажиться через те, що шифрування BitLocker було завершено, служба клієнта DHA не повідомить про те, що програма BitLocker буде активна.</span><span class="sxs-lookup"><span data-stu-id="79525-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>