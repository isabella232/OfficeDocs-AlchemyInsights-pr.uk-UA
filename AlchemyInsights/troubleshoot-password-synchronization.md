---
title: Виправлення неполадок із синхронізацією паролів
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664947"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="334e7-102">Виправлення неполадок із синхронізацією паролів</span><span class="sxs-lookup"><span data-stu-id="334e7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="334e7-103">Щоб усунути проблеми з синхронізацією паролів, запустіть цей параметр, щоб визначити, чому паролі не синхронізуються.</span><span class="sxs-lookup"><span data-stu-id="334e7-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="334e7-104">Щоб почати, перейдіть на сторінку [керування прямим синхронізацією](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="334e7-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="334e7-105">Відкрийте новий сеанс Windows PowerShell на веб-сервері Azure AD Connect і виберіть параметр " **Запуск із правами адміністратора** ".</span><span class="sxs-lookup"><span data-stu-id="334e7-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="334e7-106">Виконати віддалено або політику настроювання політики настроювання, не обмежено.</span><span class="sxs-lookup"><span data-stu-id="334e7-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="334e7-107">Запустіть майстер підключення до Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="334e7-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="334e7-108">Перейдіть на сторінку додаткові завдання, > **виправити неполадку**  >  **Далі**.</span><span class="sxs-lookup"><span data-stu-id="334e7-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="334e7-109">Натисніть кнопку **Запуск** , щоб відкрити меню виправлення неполадок PowerShell.</span><span class="sxs-lookup"><span data-stu-id="334e7-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="334e7-110">Виберіть пункт **виправляти неполадки синхронізації пароля**.</span><span class="sxs-lookup"><span data-stu-id="334e7-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="334e7-111">Ця проблема зазвичай не синхронізується з певним обліковим записом користувача.</span><span class="sxs-lookup"><span data-stu-id="334e7-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="334e7-112">**Нотатки** Синхронізація пароля не вдалася, якщо останнє успішне синхронізації пароля було якийсь час назад.</span><span class="sxs-lookup"><span data-stu-id="334e7-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="334e7-113">Докладні відомості про виправлення неполадок із синхронізацією паролів наведено в статті [Виправлення неполадок із синхронізацією гешування паролів за допомогою синхронізації Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="334e7-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>