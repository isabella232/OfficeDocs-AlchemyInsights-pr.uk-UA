---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821468"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="3ad76-102">Виправлення помилок доставки з кодом 550 5.4.1 Relay Access Denied</span><span class="sxs-lookup"><span data-stu-id="3ad76-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="3ad76-103">Ця проблема виникає під [час перевірки,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) чи дійсна адреса електронної пошти для запобігання ненадійним викликам під час входу в мережу Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ad76-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="3ad76-104">Спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="3ad76-104">Try the following:</span></span>

1. <span data-ttu-id="3ad76-105">Визначте, чи проблема характерна для всього домену або однієї адреси електронної пошти:</span><span class="sxs-lookup"><span data-stu-id="3ad76-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="3ad76-106">Увесь домен: іноді потрібно синхронізувати домен; спробуйте [вибрати для домену значення Внутрішній, а потім – на Повноважний.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="3ad76-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="3ad76-107">Одна адреса електронної пошти: іноді потрібно синхронізувати адресу; Змінення адреси проксі-сервера SMTP, а потім її повернення може допомогти.</span><span class="sxs-lookup"><span data-stu-id="3ad76-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="3ad76-108">Визначте, чи проблема характерна для групи або спільної папки.</span><span class="sxs-lookup"><span data-stu-id="3ad76-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="3ad76-109">Для деяких типів об'єктів в Azure Active Directory може знадобитися вручну створити об'єкти.</span><span class="sxs-lookup"><span data-stu-id="3ad76-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="3ad76-110">Якщо вам потрібна додаткова допомога, надішліть запит на підтримку та вкажіть обсяг проблеми (зокрема тип об'єкта, на який ви надсилаєте повідомлення), щоб ми допомогли вам краще.</span><span class="sxs-lookup"><span data-stu-id="3ad76-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>