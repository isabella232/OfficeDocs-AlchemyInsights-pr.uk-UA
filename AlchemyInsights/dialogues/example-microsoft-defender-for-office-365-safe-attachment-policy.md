---
title: Приклад політики Microsoft Defender для безпечного вкладення в Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695190"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="a0f2c-102">Приклад політики Microsoft Defender для безпечного вкладення в Office 365</span><span class="sxs-lookup"><span data-stu-id="a0f2c-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="a0f2c-103">Ці параметри дають змогу політиці під назвою " *без затримок* ", що доставляє повідомлення негайно, а потім повторно надає вкладення після того, як вони скануються:</span><span class="sxs-lookup"><span data-stu-id="a0f2c-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="a0f2c-104">**Ім'я**: без затримок</span><span class="sxs-lookup"><span data-stu-id="a0f2c-104">**Name**: No delays</span></span>
- <span data-ttu-id="a0f2c-105">**Опис**: доставляє повідомлення негайно й повторно надає вкладення після сканування.</span><span class="sxs-lookup"><span data-stu-id="a0f2c-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="a0f2c-106">**Відповідь**: виберіть параметр **динамічної доставки** .</span><span class="sxs-lookup"><span data-stu-id="a0f2c-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="a0f2c-107">Докладні відомості наведено в статті [динамічна доставка в надійних політиці вкладень](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="a0f2c-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="a0f2c-108">Розділ " **переспрямування вкладень** ": виберіть параметр, щоб **Увімкнути переспрямування**, а потім введіть адресу електронної пошти глобального адміністратора Microsoft 365, адміністратора системи безпеки або аналітика системи безпеки, які розслідуватимуть зловмисні вкладення.</span><span class="sxs-lookup"><span data-stu-id="a0f2c-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="a0f2c-109">**Застосувати до** розділу: виберіть **домен одержувача**, а потім виберіть свій домен.</span><span class="sxs-lookup"><span data-stu-id="a0f2c-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="a0f2c-110">Виберіть **Додати**, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="a0f2c-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="a0f2c-111">Завершивши, натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="a0f2c-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="a0f2c-112">Щоб отримати докладні відомості, перегляньте елементи [надійні вкладення в програмі Microsoft Defender для Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="a0f2c-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
