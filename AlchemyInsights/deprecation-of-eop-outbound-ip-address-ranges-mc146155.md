---
title: 1065 про несхвалення EOP вихідної IP-адреси rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806816"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="64fbc-102">Несхвалення вихідних діапазонів IP-адрес EOP</span><span class="sxs-lookup"><span data-stu-id="64fbc-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="64fbc-103">Ми виявили потенційну проблему з організацією, яка (якщо не виправлено від 26 жовтня 2018), може призвести до розриву потоку пошти до локальних або зовнішніх напрямків.</span><span class="sxs-lookup"><span data-stu-id="64fbc-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="64fbc-104">Як повідомлялося раніше, щоб спростити керування діапазоном IP-адрес, ми Зміцнімо діапазони IP-адрес захисту Exchange Online (EOP), які використовуються для надсилання й отримання електронної пошти за межі Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="64fbc-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="64fbc-105">Наш аналіз вказує на те, що один або кілька із зовнішніх джерел електронної пошти або пунктів призначення, настроєні в з'єднаннях пошти, не приймають з'єднання з діапазонів IP-адрес, що відображаються [тут](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="64fbc-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="64fbc-106">Дії перед 26 жовтня для забезпечення цих джерел і призначень буде приймати підключення до та від всіх [опублікованих IP-адрес EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="64fbc-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="64fbc-107">Щоб отримати докладні відомості про ці зміни, ознайомтеся з відомостями про повідомлення центру повідомлень [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)або [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="64fbc-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="64fbc-108">**Примітка**. Якщо ви раніше використовували IP-адресу або публікацію URL-адрес за допомогою HTML, XML і RSS для оновлень кінцевої точки, ви також повинні перейти до нових веб-служб для автоматизації цих типів оновлень.</span><span class="sxs-lookup"><span data-stu-id="64fbc-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="64fbc-109">Щоб отримати докладніші відомості, ознайомтеся з [категоріями кінцевих точок microsoft 365 і microsoft 365 IP-адресою та веб-службою URL-адресою](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="64fbc-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
