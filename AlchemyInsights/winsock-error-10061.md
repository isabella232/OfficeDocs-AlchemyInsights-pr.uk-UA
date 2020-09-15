---
title: Помилка 1554 Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698883"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="1f5b1-102">Помилка "Winsock 10061"</span><span class="sxs-lookup"><span data-stu-id="1f5b1-102">Winsock error 10061</span></span>

<span data-ttu-id="1f5b1-103">Цей код помилки означає, що корпорація Майкрософт не може встановити TCP-роз'єм (підключення) із цільовим хостом.</span><span class="sxs-lookup"><span data-stu-id="1f5b1-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="1f5b1-104">Скоріш за все, причиною цієї помилки є проблема з конфігурацією брандмауера.</span><span class="sxs-lookup"><span data-stu-id="1f5b1-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="1f5b1-105">Щоб вирішити цю проблему, перевірте ці параметри.</span><span class="sxs-lookup"><span data-stu-id="1f5b1-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="1f5b1-106">Перевірка конфігурації брандмауера за відомостями в [діапазонах URL-адрес і IP-адрес Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="1f5b1-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="1f5b1-107">Якщо ця помилка стосується захисту Exchange Online (EOP), ви повинні були попередньо проінформовані про змінення [IP-адрес захисту Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="1f5b1-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="1f5b1-108">Переконайтеся, що ваш постачальник послуг Інтернету (ISP) не блокує порт.</span><span class="sxs-lookup"><span data-stu-id="1f5b1-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="1f5b1-109">Перевірте настройки смарт-хоста та цільового сервера в сполуках.</span><span class="sxs-lookup"><span data-stu-id="1f5b1-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="1f5b1-110">Зверніть увагу, що корпорація Майкрософт 365 не блокує *Вхідні* підключення таким чином.</span><span class="sxs-lookup"><span data-stu-id="1f5b1-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
