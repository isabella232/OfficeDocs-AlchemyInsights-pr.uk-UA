---
title: Під час фіксації програм Microsoft 365 не вдалося знайти зв'язане повідомлення про ліцензії Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747716"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="e6e01-102">Виправлення програм Microsoft 365 "не вдалося знайти повідомлення, пов'язані з ліцензіями Office"</span><span class="sxs-lookup"><span data-stu-id="e6e01-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="e6e01-103">Якщо ви отримали це повідомлення, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="e6e01-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e6e01-104">Перевірте брандмауер, антивірусне програмне забезпечення та параметри проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e6e01-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e6e01-105">Переглянути [URL-адреси Microsoft 365 і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e6e01-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="e6e01-106">Видаліть і [Перепризначте ліцензію Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) для постраждалому користувачу.</span><span class="sxs-lookup"><span data-stu-id="e6e01-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="e6e01-107">Відкрийте програму Office і [вийдіть](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) із наявних облікових записів користувачів.</span><span class="sxs-lookup"><span data-stu-id="e6e01-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="e6e01-108">Перейдіть до параметрів Windows > **облікові**записи  >  **електронної пошти & облікових записів**і видаліть усі робочі облікові записи, окрім облікового запису, який впливає на обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="e6e01-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="e6e01-109">Перейдіть до настройок Windows > **облікові записи**для  >  **роботи або навчального закладу**, а також відключіть усі робочі облікові записи, окрім облікового запису, який впливає на нього.</span><span class="sxs-lookup"><span data-stu-id="e6e01-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="e6e01-110">Скидання стану активації Office.</span><span class="sxs-lookup"><span data-stu-id="e6e01-110">Reset the Office activation state.</span></span> <span data-ttu-id="e6e01-111">[Дізнайтеся, як це зробити](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="e6e01-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="e6e01-112">[Увійдіть](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) за допомогою облікового запису користувача, що вплинуло.</span><span class="sxs-lookup"><span data-stu-id="e6e01-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="e6e01-113">Додаткові рішення щодо виправлення неполадок наведено [в статті неліцензований продукт і помилки активації в Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="e6e01-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>