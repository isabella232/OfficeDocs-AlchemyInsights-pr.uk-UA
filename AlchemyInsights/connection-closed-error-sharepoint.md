---
title: Помилка закриття основного підключення в SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543058"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="acb11-102">Помилка "Основне підключення закрито" в SharePoint</span><span class="sxs-lookup"><span data-stu-id="acb11-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="acb11-103">Якщо з'являється повідомлення про помилку "Основне підключення закрито" в SharePoint може бути пов'язано з вилученням протоколу TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="acb11-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="acb11-104">Докладні відомості див. в таких статтях:</span><span class="sxs-lookup"><span data-stu-id="acb11-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="acb11-105">Підготовка до TLS 1.2 у Office 365 і Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="acb11-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="acb11-106">Помилки автентифікації, якщо клієнт не підтримує протокол TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="acb11-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="acb11-107">Оновлення для ввімкнення протоколів TLS 1.1 і TLS 1.2 як безпечних протоколів за замовчуванням у WindowsHTTP у Windows</span><span class="sxs-lookup"><span data-stu-id="acb11-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="acb11-108">Якщо користувачів увімкнено Windows 7, переконайтеся, що вони перевіряли [TLS Cipher Suites Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="acb11-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>