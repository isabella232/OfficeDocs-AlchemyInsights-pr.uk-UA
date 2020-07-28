---
title: Кілька об'єктів мають однакову адресу електронної пошти як особистість
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
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439706"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="4188e-102">Кілька об'єктів мають однакову адресу електронної пошти як особистість</span><span class="sxs-lookup"><span data-stu-id="4188e-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="4188e-103">**Кілька об'єктів**</span><span class="sxs-lookup"><span data-stu-id="4188e-103">**Multiple objects**</span></span>

<span data-ttu-id="4188e-104">Одна з поширених причин цієї помилки не в змозі направити Outlook Web запит на доступ належним чином у присутності кількох об'єктів, які мають однакові адреси електронної пошти, як посвідчення.</span><span class="sxs-lookup"><span data-stu-id="4188e-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="4188e-105">Щоб знайти ці об'єкти, виконайте такі команди:</span><span class="sxs-lookup"><span data-stu-id="4188e-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="4188e-106">· Get-одержувача<email address></span><span class="sxs-lookup"><span data-stu-id="4188e-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="4188e-107">· Get-користувач<email address></span><span class="sxs-lookup"><span data-stu-id="4188e-107">· Get-User <email address></span></span>

<span data-ttu-id="4188e-108">· Get-користувач <email address> -softdeleteduser</span><span class="sxs-lookup"><span data-stu-id="4188e-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="4188e-109">· Get-Контактна<email address></span><span class="sxs-lookup"><span data-stu-id="4188e-109">· Get-Contact <email address></span></span>

<span data-ttu-id="4188e-110">· Get-поштова скринька <email address> -публітека</span><span class="sxs-lookup"><span data-stu-id="4188e-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="4188e-111">· Get-поштова скринька <email address> -включаєпоштова скринька</span><span class="sxs-lookup"><span data-stu-id="4188e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="4188e-112">· Get-поштова скринька-тільки для електронної пошти <email address></span><span class="sxs-lookup"><span data-stu-id="4188e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="4188e-113">Щоб вирішити цю проблему, видаліть кілька об'єктів з одного посвідчення електронної пошти та переконайтеся, що є один об'єкт з певної посвідчення електронної пошти і що його тип одержувача є поштову скриньку користувача.</span><span class="sxs-lookup"><span data-stu-id="4188e-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="4188e-114">**Ж адреса використовується для ділових і споживчих поштових скриньок**</span><span class="sxs-lookup"><span data-stu-id="4188e-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="4188e-115">Інша причина, коли одна і та сама адреса використовується для ділових і споживчих поштових скриньок.</span><span class="sxs-lookup"><span data-stu-id="4188e-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="4188e-116">У цьому випадку користувач повинен змінити свій основний псевдонім споживача, доки кафе не підтримує цей сценарій.</span><span class="sxs-lookup"><span data-stu-id="4188e-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="4188e-117">Це постійна помилка, яка не йде без втручання.</span><span class="sxs-lookup"><span data-stu-id="4188e-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="4188e-118">Докладнішу інформацію наведено [в полі зміна адреси електронної пошти або номера телефону облікового запису Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="4188e-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>