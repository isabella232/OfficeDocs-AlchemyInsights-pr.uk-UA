---
title: 1065 вилучення ПЕРІОДУ, вихідний IP-адреса rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704618"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="e91a3-102">Вилучення діапазону вихідних IP-адрес на кінець періоду</span><span class="sxs-lookup"><span data-stu-id="e91a3-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="e91a3-103">Ми виявили потенційні проблеми з організацією, яка (якщо не виправити 26 жовтня, 2018) може розірвати потік пошти до локальної або зовнішньої призначення.</span><span class="sxs-lookup"><span data-stu-id="e91a3-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="e91a3-104">Як раніше повідомляється, для спрощення керування IP-адрес, ми консолідація Exchange Online захист (кінець періоду) IP-адреса діапазони, які використовуються для надсилання й отримання електронної пошти за межами Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e91a3-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="e91a3-105">Наш аналіз вказує на те, що один або кілька зовнішніх джерел електронної пошти або місця призначення, які ви настроїли з'єднувачі для потоку пошти, не приймає підключення з IP-адресу діапазонів показано [тут](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="e91a3-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="e91a3-106">Закон до 26 жовтня для забезпечення цих джерел і напрямків буде приймати підключення до і з усіх [опублікованих кінець періоду IP-адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="e91a3-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="e91a3-107">Щоб отримати додаткові відомості про цю зміну, будь ласка, перегляньте повідомлення центру повідомлень [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="e91a3-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="e91a3-108">**Примітка**: Якщо ви раніше використовували IP або URL публікації через HTML, XML і RSS для оновлення кінцевої точки, ви також повинні перейти на нові веб-сервіси для автоматизації цих типів оновлень.</span><span class="sxs-lookup"><span data-stu-id="e91a3-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="e91a3-109">Щоб отримати додаткові відомості див. [корпорація майкрософт 365 кінцевої точки категорій та Microsoft 365 IP-адресу та URL веб-служби](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="e91a3-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
