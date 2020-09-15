---
title: Антиспам 5.4.1 DBEB Catch-All
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717382"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="a1a6e-102">Вирішення проблем із доставкою для помилки з кодом 550 5.4.1-ретрансляцією відмовлено в доступі</span><span class="sxs-lookup"><span data-stu-id="a1a6e-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="a1a6e-103">Ця проблема виникає, [Якщо перевірити, чи є адреса електронної пошти дійсною, щоб запобігти bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) під час входу в мережу Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a1a6e-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="a1a6e-104">Виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="a1a6e-104">Try the following:</span></span>

1. <span data-ttu-id="a1a6e-105">Визначення того, чи ця проблема стосується всього домену або однієї адреси електронної пошти:</span><span class="sxs-lookup"><span data-stu-id="a1a6e-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="a1a6e-106">Увесь домен: іноді потрібно синхронізувати домен; Спробуйте [настроїти домен на внутрішній, а потім знову на важливий](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="a1a6e-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="a1a6e-107">Єдина адреса електронної пошти: іноді потрібно синхронізувати адресу. Щоб змінити адресу проксі-сервера SMTP, а потім знову змінити його, може допомогти.</span><span class="sxs-lookup"><span data-stu-id="a1a6e-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="a1a6e-108">Визначення того, чи ця проблема стосується групи або спільної папки.</span><span class="sxs-lookup"><span data-stu-id="a1a6e-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="a1a6e-109">Для деяких типів об'єктів, можливо, потрібно вручну створити в Лазурому Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a1a6e-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="a1a6e-110">Якщо вам потрібна додаткова довідка, відкрийте квиток підтримки та вкажіть область цієї проблеми (включно з типом об'єкта, який ви надсилаєте), щоб ми могли краще допомогти вам.</span><span class="sxs-lookup"><span data-stu-id="a1a6e-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>