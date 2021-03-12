---
title: Пошук і видалення повідомлень електронної пошти в організації
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750021"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="14b5d-102">Пошук і видалення повідомлень електронної пошти в організації</span><span class="sxs-lookup"><span data-stu-id="14b5d-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="14b5d-103">Виконайте наведені нижче кроки.</span><span class="sxs-lookup"><span data-stu-id="14b5d-103">Follow these steps:</span></span>

1. <span data-ttu-id="14b5d-104">Якщо ви не є глобальним адміністратором, щоб знайти повідомлення, які потрібно додати до вашого облікового запису, до рольової **групи «Диспетчер** Витребування» або **ролі керування відповідністю**.</span><span class="sxs-lookup"><span data-stu-id="14b5d-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="14b5d-105">Щоб видалити повідомлення, потрібно приєднатися до рольової групи " **Керування організацією** " або " **Пошук і очищення**".</span><span class="sxs-lookup"><span data-stu-id="14b5d-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="14b5d-106">Дозволи для цих ролей призначено в [центрі відповідності & безпеки.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="14b5d-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="14b5d-107">[Створіть пошук вмісту](https://docs.microsoft.com/office365/securitycompliance/content-search) , щоб знайти повідомлення, яке потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="14b5d-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="14b5d-108">[Підключення до центру безпеки та відповідності & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="14b5d-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="14b5d-109">Якщо ви використовуєте МЗС, ознайомтеся з наведеними нижче вказівками: [підключення до центру безпеки & відповідність PowerShell за допомогою багатофакторної автентифікації](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="14b5d-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="14b5d-110">Видаліть повідомлення: запустіть `New-ComplianceSearchAction` командлет, щоб видалити повідомлення.</span><span class="sxs-lookup"><span data-stu-id="14b5d-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="14b5d-111">Видалені повідомлення переміщуються до папки «Відновлювані елементи» користувача.</span><span class="sxs-lookup"><span data-stu-id="14b5d-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="14b5d-112">У полі приклад виберіть команду [крок 3: видалення повідомлення.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="14b5d-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
