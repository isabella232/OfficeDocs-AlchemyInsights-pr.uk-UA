---
title: Запуск діагностики пам'яті Windows у Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358290"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="77e44-102">Запуск діагностики пам'яті Windows у Windows 10</span><span class="sxs-lookup"><span data-stu-id="77e44-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="77e44-103">Якщо Windows і програми на ПК аварійно завершує роботу, заморозять або діють у нестабільному режимі, можливо, виникли проблеми з пам'яттю ПК (ОЗП).</span><span class="sxs-lookup"><span data-stu-id="77e44-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="77e44-104">Можна запустити діагностику пам'яті Windows, щоб перевірити наявність проблем із оперативною пам'яттю ПК.</span><span class="sxs-lookup"><span data-stu-id="77e44-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="77e44-105">У полі пошуку на панелі завдань введіть **діагностику пам'яті**, а потім виберіть **діагностику пам'яті Windows**.</span><span class="sxs-lookup"><span data-stu-id="77e44-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="77e44-106">Для запуску діагностики комп'ютер потрібно перезавантажити.</span><span class="sxs-lookup"><span data-stu-id="77e44-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="77e44-107">Ви маєте можливість негайно перезавантажити комп'ютер (будь ласка, збережіть свою роботу і закрийте відкриті документи та електронну пошту першими) або заплануйте діагностику для автоматичного запуску наступного разу, коли комп'ютер перезавантажиться:</span><span class="sxs-lookup"><span data-stu-id="77e44-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Діагностики пам'яті Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="77e44-109">Під час перезавантаження комп'ютера **засіб діагностики пам'яті Windows** буде запущено автоматично.</span><span class="sxs-lookup"><span data-stu-id="77e44-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="77e44-110">Стан і прогрес буде відображатися в міру виконання діагностики, і у вас є можливість скасувати діагностику, натиснувши клавішу **ESC** на клавіатурі.</span><span class="sxs-lookup"><span data-stu-id="77e44-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="77e44-111">Коли діагностику завершено, Windows почне нормально.</span><span class="sxs-lookup"><span data-stu-id="77e44-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="77e44-112">Відразу після перезавантаження, коли робочий стіл з'явиться, з'явиться сповіщення (поруч із піктограмою **центру підтримки** на панелі завдань), щоб вказати, чи були виявлені помилки в пам'яті.</span><span class="sxs-lookup"><span data-stu-id="77e44-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="77e44-113">Наприклад,</span><span class="sxs-lookup"><span data-stu-id="77e44-113">For example:</span></span>

<span data-ttu-id="77e44-114">Ось піктограма Центру підтримки:</span><span class="sxs-lookup"><span data-stu-id="77e44-114">Here's the Action Center icon:</span></span> ![Піктограма Центру підтримки](media/action-center-icon.png) 

<span data-ttu-id="77e44-116">І приклад повідомлення:</span><span class="sxs-lookup"><span data-stu-id="77e44-116">And a sample notification:</span></span> ![Немає помилок пам'яті](media/no-memory-errors.png)

<span data-ttu-id="77e44-118">Якщо ви пропустили сповіщення, можна вибрати піктограму **центру підтримки** на панелі завдань, щоб відобразити **центр підтримки** та переглянути прокручуване список сповіщень.</span><span class="sxs-lookup"><span data-stu-id="77e44-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="77e44-119">Щоб переглянути докладні відомості, введіть **подію** в поле пошуку на панелі завдань, а потім виберіть пункт **Перегляд подій**.</span><span class="sxs-lookup"><span data-stu-id="77e44-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="77e44-120">У лівій області **перегляду подій**перейдіть до **журналу Windows > системи**.</span><span class="sxs-lookup"><span data-stu-id="77e44-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="77e44-121">В області праворуч виконайте пошук у списку під час перегляду **вихідної** колонки, доки не побачите події з вихідним значенням у **запам'ятовидіагностика-результати**.</span><span class="sxs-lookup"><span data-stu-id="77e44-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="77e44-122">Виділіть кожну таку подію та перегляньте інформацію про результат у полі на вкладці **загальні** під списком.</span><span class="sxs-lookup"><span data-stu-id="77e44-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
