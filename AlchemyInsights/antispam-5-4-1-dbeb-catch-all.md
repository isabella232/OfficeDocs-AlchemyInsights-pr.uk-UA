---
title: Антиспам 5.4.1 DBEB зловити-все
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672454"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="706c8-102">Вирішення проблем із доставкою код помилки 550 5.4.1 ретранслятор доступ заборонено</span><span class="sxs-lookup"><span data-stu-id="706c8-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="706c8-103">Ця проблема виникає під час [перевірки, щоб побачити, якщо адреса електронної пошти дійсний для запобігання](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) під час переходу до мережі Office 365.</span><span class="sxs-lookup"><span data-stu-id="706c8-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="706c8-104">Спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="706c8-104">Try the following:</span></span>

1. <span data-ttu-id="706c8-105">Визначте, чи проблема стосується всього домену або одну адресу електронної пошти:</span><span class="sxs-lookup"><span data-stu-id="706c8-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="706c8-106">Увесь домен: інколи потрібно синхронізувати домен; Спробуйте [настроїти домен на внутрішній, а потім повернутися до основного](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="706c8-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="706c8-107">Єдина адреса електронної пошти: іноді адреса повинна бути синхронізована; зміна адреси SMTP-проксі-сервера, а потім змінити його назад може допомогти.</span><span class="sxs-lookup"><span data-stu-id="706c8-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="706c8-108">Визначте, чи проблема специфічна для групи або спільних папок.</span><span class="sxs-lookup"><span data-stu-id="706c8-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="706c8-109">Для деяких типів об'єктів, можливо, доведеться вручну створити в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="706c8-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="706c8-110">Якщо вам потрібна додаткова допомога, будь ласка, відкрийте квиток підтримки і вкажіть сферу цього питання (включаємо тип об'єкту, який ви посилаєте), щоб ми могли допомогти вам краще.</span><span class="sxs-lookup"><span data-stu-id="706c8-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>