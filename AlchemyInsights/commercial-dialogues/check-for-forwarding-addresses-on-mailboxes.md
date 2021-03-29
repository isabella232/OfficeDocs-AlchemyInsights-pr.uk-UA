---
title: Перевірка адреси пересилання в поштових скриньках
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403332"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="f5462-102">Перевірка адреси пересилання в поштових скриньках</span><span class="sxs-lookup"><span data-stu-id="f5462-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="f5462-103">Іноді хакери пересилають електронні листи самостійно, тому спочатку ми перевіримо адреси й правила пересилання в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="f5462-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="f5462-104">Потім ми перевіримо контрольні журнали.</span><span class="sxs-lookup"><span data-stu-id="f5462-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="f5462-105">Ось як перевірити адреси пересилання:</span><span class="sxs-lookup"><span data-stu-id="f5462-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="f5462-106">Виберіть **елемент**  >  **Активні користувачі.**</span><span class="sxs-lookup"><span data-stu-id="f5462-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="f5462-107">Виберіть користувача, обліковий запис якого зламали.</span><span class="sxs-lookup"><span data-stu-id="f5462-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="f5462-108">У розгорнутому меню, що з'явиться, розгорніть елемент Параметри пошти **,** а потім виберіть Редагувати **для** параметра **Пересилання електронної пошти**.</span><span class="sxs-lookup"><span data-stu-id="f5462-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="f5462-109">Видаліть не розпізнані адреси пересилання.</span><span class="sxs-lookup"><span data-stu-id="f5462-109">Remove any forwarding addresses you don't recognize.</span></span>