---
title: Виправлення 0x8004de40 oneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649769"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8e536-102">Виправлення 0x8004de40 oneDrive</span><span class="sxs-lookup"><span data-stu-id="8e536-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8e536-103">Якщо під час роботи з Windows 7 з'являється таке повідомлення про помилку, оновіть windows, щоб активувати [протоколИ TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)як безпечні протоколи за замовчуванням у WindowsHTTP.</span><span class="sxs-lookup"><span data-stu-id="8e536-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="8e536-104">Якщо використовується Windows 10 і з'являється повідомлення про помилку 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8e536-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8e536-105">Перезавантажте комп'ютер, на який це вплине, підключившись до домену Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="8e536-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8e536-106">Якщо перезавантаження не допомогло вирішити проблему, повторно під'єдайте свій пристрій з Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8e536-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8e536-107">**Примітка.** Ці кроки потрібно розташувати в корпоративній мережі.</span><span class="sxs-lookup"><span data-stu-id="8e536-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8e536-108">Не виконуйте ці дії, коли не підключено до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="8e536-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="8e536-109">Відкрийте командний рядок у режимі адміністратора, натиснувши **кнопку** Пуск , клацніть правою кнопкою **миші** пункт Командний рядок і виберіть **команду Запустити із правами адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="8e536-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="8e536-110">Введіть *dsregcmd /leave і* натисніть клавішу **Enter.**</span><span class="sxs-lookup"><span data-stu-id="8e536-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="8e536-111">Після завершення введіть *dsregcmd /join і* натисніть **клавішу Enter.**</span><span class="sxs-lookup"><span data-stu-id="8e536-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="8e536-112">Коли завершите, закрийте командний рядок.</span><span class="sxs-lookup"><span data-stu-id="8e536-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="8e536-113">Перезавантажте комп'ютер і ввійдіть у OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8e536-113">Reboot the computer, and log into OneDrive.</span></span>