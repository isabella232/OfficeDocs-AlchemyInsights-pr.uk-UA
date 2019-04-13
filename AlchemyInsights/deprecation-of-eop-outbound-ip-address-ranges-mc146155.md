---
title: 1065 несхвалення EOP Вихідна IP-адреса rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858117"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="04c8e-102">Несхвалення EOP вихідне Вихідна IP-адреса</span><span class="sxs-lookup"><span data-stu-id="04c8e-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="04c8e-103">Це свідчить потенційна проблема з вашої організації, які (якщо не виправити, 26 жовтня 2018) може порушити потік пошти локальні або зовнішні джерела.</span><span class="sxs-lookup"><span data-stu-id="04c8e-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="04c8e-104">Як раніше передано спростити IP адреса діапазон керування, ми ти консолідації діапазони Exchange Online захисту (EOP) IP-адрес, які використовуються для надсилання й отримання електронної пошти за межами Office 365.</span><span class="sxs-lookup"><span data-stu-id="04c8e-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="04c8e-105">Наш аналіз показує, що подані зовнішню поштову джерела або місця, які ви налаштували у роз'ємах потік пошти не приймає підключення з на IP адреса діапазони показано [тут](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="04c8e-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="04c8e-106">Виступати перед 26 жовтня для забезпечення цих джерел та напрямків буде приймати з'єднання і від всіх [опубліковані EOP IP-адрес](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="04c8e-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="04c8e-107">Щоб отримати додаткові відомості про цю зміну будь ласка, дивіться центрі повідомлень повідомлення з [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="04c8e-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="04c8e-108">**Примітка**: Якщо ви раніше використовували IP або URL публікації за допомогою HTML, XML та RSS для кінцевої точки оновлень, також повинні міграцією до нових веб-сервісів для автоматизації ці типи оновлень.</span><span class="sxs-lookup"><span data-stu-id="04c8e-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="04c8e-109">Докладніше перегляньте [Office 365 кінцевої точки категорії та Office 365 IP-адреси та URL-адресу веб-служби](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="04c8e-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
