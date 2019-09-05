---
title: S/MIME у програмі Outlook на веб-сайті
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752881"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="6dd00-102">Шифрувати повідомлення електронної пошти в Outlook</span><span class="sxs-lookup"><span data-stu-id="6dd00-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="6dd00-103">Office 365 повідомлення шифрування, побудована на Microsoft Azure прав керування (Azure RMS), який входить до складу Azure відомості про захист.</span><span class="sxs-lookup"><span data-stu-id="6dd00-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="6dd00-104">Якщо ваша підписка включає керування правами Azure або захист інформації в Azure, **не потрібно виконувати жодних дій, щоб вручну увімкнути або активувати** службу керування правами.</span><span class="sxs-lookup"><span data-stu-id="6dd00-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="6dd00-105">На основі відгуків клієнтів ми більше не вмикаємо правила потоку Exchange Mail, щоб автоматично шифрувати вихідне повідомлення електронної пошти, що містить певний тип конфіденційної інформації у вашому клієнті за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="6dd00-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="6dd00-106">Замість цього, ми надаємо докладні інструкції про те, як ви можете зробити це самі.</span><span class="sxs-lookup"><span data-stu-id="6dd00-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="6dd00-107">Додаткові відомості про створення правила транспортування для шифрування конфіденційної інформації наведено в [цій статті](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="6dd00-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="6dd00-108">У разі використання Outlook на веб-сайті (раніше **OWA**): при складанні повідомлення електронної пошти, просто натисніть кнопку **захистити** в owa.</span><span class="sxs-lookup"><span data-stu-id="6dd00-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="6dd00-109">Це застосує дозвіл "не пересилати".</span><span class="sxs-lookup"><span data-stu-id="6dd00-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="6dd00-110">Натисніть **змінити дозвіл** і виберіть **шифрувати** , щоб зашифрувати повідомлення.</span><span class="sxs-lookup"><span data-stu-id="6dd00-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="6dd00-111">Якщо використовується **клієнт Outlook**: надіслати зашифроване повідомлення з Outlook 2013 або 2016 або Outlook 2016 для Mac, виберіть **Параметри** > **дозволи**, а потім виберіть потрібний параметр захисту.</span><span class="sxs-lookup"><span data-stu-id="6dd00-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="6dd00-112">Щоб **автоматично шифрувати всі повідомлення** , надіслані певним одержувачам або зовнішнім партнерським організаціям, потрібно створити правило транспортування пошти в центрі адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dd00-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="6dd00-113">Докладні інструкції наведено в [цій статті підтримки](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="6dd00-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

