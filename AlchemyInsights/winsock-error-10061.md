---
title: 1554 Winsock помилка 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766190"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="265ec-102">Winsock помилка 10061</span><span class="sxs-lookup"><span data-stu-id="265ec-102">Winsock error 10061</span></span>

<span data-ttu-id="265ec-103">Цей код помилки означає, що корпорація Майкрософт не може встановити TCP-сокет (підключення) з цільового хоста.</span><span class="sxs-lookup"><span data-stu-id="265ec-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="265ec-104">Найбільш вірогідною причиною цієї помилки є проблема з конфігурацією брандмауера.</span><span class="sxs-lookup"><span data-stu-id="265ec-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="265ec-105">Щоб вирішити цю проблему, перевірте, чи ці параметри:</span><span class="sxs-lookup"><span data-stu-id="265ec-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="265ec-106">Перевірте конфігурацію брандмауера з відомостями в [Microsoft 365 URL-адрес і діапазонів IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="265ec-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="265ec-107">Якщо повідомлення про помилку, специфічні для Exchange Online захисту (кінець періоду), ви повинні були раніше повідомлені зміни в [Exchange Online захист IP-адрес](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="265ec-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="265ec-108">Переконайтеся, що ваш інтернет-провайдер (ISP) не блокує порт.</span><span class="sxs-lookup"><span data-stu-id="265ec-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="265ec-109">Перевірте настройки смарт-хоста та цільового сервера в з'єднувачів.</span><span class="sxs-lookup"><span data-stu-id="265ec-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="265ec-110">Зверніть увагу, що Microsoft 365 не блокує *Вхідні* підключення таким чином.</span><span class="sxs-lookup"><span data-stu-id="265ec-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
