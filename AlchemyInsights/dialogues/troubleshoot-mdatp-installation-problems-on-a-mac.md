---
title: Виправлення неполадок інсталяції MDATP на комп'ютері Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696100"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="abe6c-102">Виправлення неполадок інсталяції MDATP на комп'ютері Mac</span><span class="sxs-lookup"><span data-stu-id="abe6c-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="abe6c-103">Якщо не вдалося виконати інсталяцію вручну, на сторінці « **зведення** » майстра інсталяції відображається таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="abe6c-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="abe6c-104">"Під час інсталяції сталася помилка".</span><span class="sxs-lookup"><span data-stu-id="abe6c-104">"An error occurred during installation.</span></span> <span data-ttu-id="abe6c-105">Помилка інсталятора виявила помилку, яка призвела до помилки інсталяції.</span><span class="sxs-lookup"><span data-stu-id="abe6c-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="abe6c-106">Зверніться до виробника програмного забезпечення, щоб отримати допомогу. "</span><span class="sxs-lookup"><span data-stu-id="abe6c-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="abe6c-107">У разі розгортання для MDM на сторінці відображається Загальна помилка інсталяції.</span><span class="sxs-lookup"><span data-stu-id="abe6c-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="abe6c-108">Хоча ми не відображаємо точні помилки для кінцевого користувача, ми зберігаємо файл журналу з прогресом інсталяції в **/Library/logs/Microsoft/mdatp/Install.log**.</span><span class="sxs-lookup"><span data-stu-id="abe6c-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="abe6c-109">Кожний сеанс інсталяції додається до цього файлу журналу.</span><span class="sxs-lookup"><span data-stu-id="abe6c-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="abe6c-110">Щоб вивести лише останній сеанс інсталяції, використовуйте її `sed` .</span><span class="sxs-lookup"><span data-stu-id="abe6c-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="abe6c-111">Докладні відомості наведено в статті [Виправлення неполадок із інсталяцією для системи захисту від захисника Microsoft для Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="abe6c-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
