---
title: S/MIME в Інтернет-версії Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772319"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="44c41-102">Шифрування повідомлень електронної пошти в Outlook</span><span class="sxs-lookup"><span data-stu-id="44c41-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="44c41-103">Шифрування повідомлень Microsoft 365 створено на основі керування правами доступу до інформації Microsoft Azure (Azure RMS), що входить до складу інформаційного захисту від Лазур.</span><span class="sxs-lookup"><span data-stu-id="44c41-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="44c41-104">Якщо ваша Передплата включає в себе керування невізуаними правами або лазуровий захист інформації, **вам не потрібно виконувати жодні дії, щоб вмикати або активувати** службу керування правами.</span><span class="sxs-lookup"><span data-stu-id="44c41-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="44c41-105">На основі відгуків клієнтів, ми більше не зможемо активувати правила передавання пошти Exchange, щоб автоматично шифрувати вихідне повідомлення електронної пошти з певним типом конфіденційної інформації в клієнті за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="44c41-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="44c41-106">Натомість ми надаємо докладні вказівки про те, як це можна зробити самостійно.</span><span class="sxs-lookup"><span data-stu-id="44c41-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="44c41-107">Щоб отримати додаткові відомості про те, як створити правило транспортування для шифрування конфіденційної інформації, ознайомтеся з [цією статтею](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="44c41-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="44c41-108">Якщо ви використовуєте Інтернет-версію Outlook (колишня **WA**): під час створення повідомлення електронної пошти, просто натисніть кнопку **захистити** у owa.</span><span class="sxs-lookup"><span data-stu-id="44c41-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="44c41-109">Для цього буде застосовано дозвіл "Do Not пересилання".</span><span class="sxs-lookup"><span data-stu-id="44c41-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="44c41-110">Натисніть кнопку **змінити дозвіл** , а потім виберіть команду **Зашифрувати** , щоб зашифрувати повідомлення.</span><span class="sxs-lookup"><span data-stu-id="44c41-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="44c41-111">Якщо використовується **клієнт Outlook**: щоб відправити зашифроване повідомлення з Outlook 2013 або 2016 або Outlook 2016 для Mac, виберіть пункт **Options**  >  **дозволи**для параметрів, а потім виберіть потрібний параметр захисту.</span><span class="sxs-lookup"><span data-stu-id="44c41-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="44c41-112">Щоб **автоматично шифрувати всі повідомлення електронної пошти** , надіслані певним одержувачам або зовнішнім організаціям-партнерам, потрібно створити правило транспортування пошти в центрі адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="44c41-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="44c41-113">Докладні вказівки наведено в [цій статті підтримки](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="44c41-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

