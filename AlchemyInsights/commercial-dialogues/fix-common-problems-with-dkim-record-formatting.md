---
title: Виправлення поширених проблем із форматуванням запису DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750752"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="51ee5-102">Виправлення поширених проблем із форматуванням запису DKIM</span><span class="sxs-lookup"><span data-stu-id="51ee5-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="51ee5-103">Більшість проблем із настроюванням DKIM пов'язані з неправильними записами DNS.</span><span class="sxs-lookup"><span data-stu-id="51ee5-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="51ee5-104">Щоб виправити проблеми з настроюванням DKIM, переконайтеся, що запис DKIM CNAME (**не** запис txt) відформатовано правильно.</span><span class="sxs-lookup"><span data-stu-id="51ee5-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="51ee5-105">Щоб отримати докладніші відомості, Дізнайтеся, [що потрібно зробити, щоб вручну налаштувати DKIM в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="51ee5-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="51ee5-106">Якщо вам потрібна Довідка з записів DNS загалом, перегляньте статтю [створення записів DNS на сайті будь-якого постачальника послуг розміщення DNS для Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="51ee5-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="51ee5-107">Створивши або оновіть записи DNS DKIM у службі розміщення DNS для свого домену, необхідно зачекати, доки записи DNS потрібно буде розповсюдити.</span><span class="sxs-lookup"><span data-stu-id="51ee5-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
