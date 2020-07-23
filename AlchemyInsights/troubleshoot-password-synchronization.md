---
title: Виправлення неполадок синхронізації паролів
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387898"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c0827-102">Виправлення неполадок синхронізації паролів</span><span class="sxs-lookup"><span data-stu-id="c0827-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c0827-103">Щоб вирішити проблеми з синхронізацією паролів, почніть з використання цього сад підключення виправлення неполадок завдання, щоб визначити, чому паролі не синхронізуються.</span><span class="sxs-lookup"><span data-stu-id="c0827-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="c0827-104">Для початку перейдіть до [керування прямою синхронізацією](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="c0827-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="c0827-105">Відкрийте новий сеанс Windows PowerShell на сервері Azure AD-підключення та виберіть параметр запуск із **правами адміністратора** .</span><span class="sxs-lookup"><span data-stu-id="c0827-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c0827-106">Запустіть Set-виконання політики, Пульс, або набір-виконання політики необмежений.</span><span class="sxs-lookup"><span data-stu-id="c0827-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="c0827-107">Запустіть майстер Azure AD-підключення.</span><span class="sxs-lookup"><span data-stu-id="c0827-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c0827-108">Перейдіть на сторінку додаткових завдань > **Виправлення неполадок**  >  **Далі**.</span><span class="sxs-lookup"><span data-stu-id="c0827-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="c0827-109">Виберіть **запустити** , щоб відкрити меню виправлення неполадок PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c0827-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="c0827-110">Виберіть **Виправлення неполадок, синхронізація пароля**.</span><span class="sxs-lookup"><span data-stu-id="c0827-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="c0827-111">Зазвичай, це не синхронізація пароля для певного облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="c0827-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="c0827-112">**Нотатки** Не вдається виконати синхронізацію паролів, якщо остання успішна синхронізація пароля була деякий час назад.</span><span class="sxs-lookup"><span data-stu-id="c0827-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="c0827-113">Щоб дізнатися більше про виправлення неполадок синхронізація пароля [, див.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="c0827-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>