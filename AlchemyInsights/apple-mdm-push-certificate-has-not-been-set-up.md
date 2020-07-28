---
title: Apple MDM Push сертифікат не настроєно
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440006"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="35066-102">Apple MDM Push сертифікат не настроєно</span><span class="sxs-lookup"><span data-stu-id="35066-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="35066-103">Сертифікат Apple MDM Push (також відомий як сертифікат служби Push-сповіщень Apple (APNS)) не настроєно для передплати.</span><span class="sxs-lookup"><span data-stu-id="35066-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="35066-104">Без налаштування Apple MDM Push сертифікат, ви не можете зареєструвати і керувати iOS і Mac OS пристроїв.</span><span class="sxs-lookup"><span data-stu-id="35066-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="35066-105">Після того, як додати сертифікат InTune, користувачі можуть інсталювати програму "портал компанії", щоб зареєструвати свої пристрої iOS.</span><span class="sxs-lookup"><span data-stu-id="35066-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="35066-106">Виберіть **"я згоден".**</span><span class="sxs-lookup"><span data-stu-id="35066-106">Select **"I agree."**</span></span> <span data-ttu-id="35066-107">щоб надати корпорації Майкрософт дозвіл на надсилання даних до Apple.</span><span class="sxs-lookup"><span data-stu-id="35066-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="35066-108">Виберіть **завантажити КСВ** запит на підписування сертифікат, необхідний для створення сертифіката Apple MDM Push.</span><span class="sxs-lookup"><span data-stu-id="35066-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="35066-109">Файл використовується для запиту сертифіката довірчий зв'язок з порталу сертифікатів Apple Push.</span><span class="sxs-lookup"><span data-stu-id="35066-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="35066-110">Виберіть **створити ваш MDM Push сертифікат** , щоб перейти на порталі Apple Push сертифікатів.</span><span class="sxs-lookup"><span data-stu-id="35066-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="35066-111">Увійдіть у компанію Apple ID, а потім виберіть **створити сертифікат**.</span><span class="sxs-lookup"><span data-stu-id="35066-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="35066-112">Виберіть **пункт вибрати файл**, перейдіть до файлу запиту цифрового підпису сертифіката, а потім виберіть **завантажити**.</span><span class="sxs-lookup"><span data-stu-id="35066-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="35066-113">На сторінці підтвердження виберіть **завантажити** , щоб завантажити файл сертифіката (. pem), і збережіть файл локально.</span><span class="sxs-lookup"><span data-stu-id="35066-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="35066-114">**Примітки**: сертифікат пов'язаний з Apple ID, що використовується для його створення.</span><span class="sxs-lookup"><span data-stu-id="35066-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="35066-115">Рекомендовано використовувати компанію Apple ID для керування завданнями та переконайтеся, що поштова скринька контролюється кількома особами або за допомогою списку розсилки.</span><span class="sxs-lookup"><span data-stu-id="35066-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="35066-116">Ніколи не користуйтеся персональним ідентифікатором Apple ID.</span><span class="sxs-lookup"><span data-stu-id="35066-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="35066-117">Використовуйте той же Apple ID, щоб оновити Apple Push сертифікат кожні 12 місяців.</span><span class="sxs-lookup"><span data-stu-id="35066-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="35066-118">Введіть ІДЕНТИФІКАТОР Apple, який використовується для створення сертифіката Apple MDM Push.</span><span class="sxs-lookup"><span data-stu-id="35066-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="35066-119">Запишіть цей ІДЕНТИФІКАТОР як нагадування, коли потрібно оновити сертифікат.</span><span class="sxs-lookup"><span data-stu-id="35066-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="35066-120">Перейдіть до файлу сертифіката (. pem), виберіть **Відкрити**, а потім виберіть **завантажити**.</span><span class="sxs-lookup"><span data-stu-id="35066-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="35066-121">За допомогою сертифіката Push InTune можна зареєструвати та керувати пристроями Apple.</span><span class="sxs-lookup"><span data-stu-id="35066-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>