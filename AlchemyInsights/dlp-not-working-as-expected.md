---
title: ЗВД не працює належним чином
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977459"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="0a20d-102">ЗВД не працює належним чином</span><span class="sxs-lookup"><span data-stu-id="0a20d-102">DLP not working as expected</span></span>

<span data-ttu-id="0a20d-103">**Важливо**: у ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються доступними – будь ласка, відвідайте [тимчасові функції SharePoint Online](https://aka.ms/ODSPAdjustments) для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="0a20d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="0a20d-104">**Налаштування ЗВД**</span><span class="sxs-lookup"><span data-stu-id="0a20d-104">**Setting up DLP**</span></span>

<span data-ttu-id="0a20d-105">У вас виникли проблеми з **запобігання втрати даних (звд)** в Office 365 не працює належним чином?</span><span class="sxs-lookup"><span data-stu-id="0a20d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="0a20d-106">Якщо це так, переконайтеся, що ваша **політика звд** настроєно належним чином, і що дані, містить те, **що, якщо** вона шукає.</span><span class="sxs-lookup"><span data-stu-id="0a20d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="0a20d-107">ЗВД правила дає змогу виявляти та захищати конфіденційну інформацію в організації.</span><span class="sxs-lookup"><span data-stu-id="0a20d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="0a20d-108">Щоб налаштувати ЗВД політики, скористайтеся інформацією [тут](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="0a20d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="0a20d-109">**Що шукати ЗВД політики**</span><span class="sxs-lookup"><span data-stu-id="0a20d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="0a20d-110">Під час використання **вбудованих типів конфіденційної інформації** в Office 365 безпеки та комплаєнсу центр, звд політики, знайдіть конкретні шаблони та елементи, під час виявлення цих чутливих типів.</span><span class="sxs-lookup"><span data-stu-id="0a20d-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="0a20d-111">**Вбудовані типи конфіденційних даних**</span><span class="sxs-lookup"><span data-stu-id="0a20d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="0a20d-112">Відомості про вбудовані типи конфіденційних даних і те, що політика ЗВД шукає при виявленні чутливого типу, див.: [які типи конфіденційної інформації шукати](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="0a20d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="0a20d-113">**Користувацькі типи конфіденційних відомостей**</span><span class="sxs-lookup"><span data-stu-id="0a20d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="0a20d-114">Якщо ви намагаєтесь створити спеціальні типи конфіденційних відомостей, використайте таку статтю, щоб отримати відомості про те, як створити користувацький чутливий тип: [створити користувацький тип конфіденційної інформації](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0a20d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="0a20d-115">**Перевірка ЗВД політика**</span><span class="sxs-lookup"><span data-stu-id="0a20d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="0a20d-116">Щоб перевірити дані за допомогою вбудованого або настроюваного типу даних делікатного характеру, скористайтеся параметром **Test Type** **у розділі** > **типи конфіденційних**відомостей.</span><span class="sxs-lookup"><span data-stu-id="0a20d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="0a20d-117">Щоб [отримати додаткові відомості див.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="0a20d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="0a20d-118">**Звіти**</span><span class="sxs-lookup"><span data-stu-id="0a20d-118">**Reports**</span></span>
  
- <span data-ttu-id="0a20d-119">Отримуйте конфіденційні аналітичні дані за допомогою [звітів звд.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="0a20d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="0a20d-120">Ознайомтеся з конкретними відомостями про подію у [звіті про інцидент](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="0a20d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
