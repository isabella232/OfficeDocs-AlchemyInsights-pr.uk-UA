---
title: Запуск засобу діагностики пам'яті Windows у Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826688"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="fecc5-102">Запуск засобу діагностики пам'яті Windows у Windows 10</span><span class="sxs-lookup"><span data-stu-id="fecc5-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="fecc5-103">Якщо Windows і програми на ПК аварійно завершують роботу, закріплюються або виконуються нестабільно, можливо, виникнуть проблеми з пам'яттю ПК (ОЗП).</span><span class="sxs-lookup"><span data-stu-id="fecc5-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="fecc5-104">Ви можете запустити засіб діагностики пам'яті Windows, щоб перевірити наявність проблем із оперативною пам'яттю ПК.</span><span class="sxs-lookup"><span data-stu-id="fecc5-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="fecc5-105">У полі пошуку на панелі завдань введіть "Діагностика **пам'яті"**, а потім виберіть пункт Діагностика **пам'яті Windows**.</span><span class="sxs-lookup"><span data-stu-id="fecc5-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="fecc5-106">Щоб запустити діагностику, ПК потрібно перезавантажити.</span><span class="sxs-lookup"><span data-stu-id="fecc5-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="fecc5-107">Можна відразу перезапустити програму (спочатку збережіть свою роботу та закрийте відкриті документи та повідомлення електронної пошти) або заплануйте автоматичний запуск діагностики під час наступного перезавантаження ПК.</span><span class="sxs-lookup"><span data-stu-id="fecc5-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Діагностика пам'яті Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="fecc5-109">Коли комп'ютер перезавантажиться, засіб **діагностики пам'яті Windows** запуститься автоматично.</span><span class="sxs-lookup"><span data-stu-id="fecc5-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="fecc5-110">Стан і перебіг виконання відображатимуться під час запуску діагностики, а ви можете скасувати діагностики, натиснувши клавішу **Esc** на клавіатурі.</span><span class="sxs-lookup"><span data-stu-id="fecc5-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="fecc5-111">Коли діагностика завершиться, Windows завантажиться у звичайний режим.</span><span class="sxs-lookup"><span data-stu-id="fecc5-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="fecc5-112">Коли робочий стіл відобразиться, одразу після перезавантаження  з'явиться сповіщення (біля піктограми Центру підтримки на панелі завдань), щоб указати, чи знайдено всі помилки пам'яті.</span><span class="sxs-lookup"><span data-stu-id="fecc5-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="fecc5-113">Наприклад:</span><span class="sxs-lookup"><span data-stu-id="fecc5-113">For example:</span></span>

<span data-ttu-id="fecc5-114">Ось піктограма Центру підтримки:</span><span class="sxs-lookup"><span data-stu-id="fecc5-114">Here's the Action Center icon:</span></span> ![Піктограма центру підтримки](media/action-center-icon.png) 

<span data-ttu-id="fecc5-116">І зразок сповіщення:</span><span class="sxs-lookup"><span data-stu-id="fecc5-116">And a sample notification:</span></span> ![Помилки пам'яті відсутні](media/no-memory-errors.png)

<span data-ttu-id="fecc5-118">Якщо ви пропустили сповіщення,  на панелі завдань клацніть піктограму  Центру підтримки, щоб відобразити центр підтримки та переглянути список сповіщень, які можна прокручувати.</span><span class="sxs-lookup"><span data-stu-id="fecc5-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="fecc5-119">Щоб переглянути докладні відомості, **введіть** подію в поле пошуку на панелі завдань, а потім виберіть **пункт Перегляд подій**.</span><span class="sxs-lookup"><span data-stu-id="fecc5-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="fecc5-120">В області **"Перегляд подій"** ліворуч перейдіть до пункту Журнали **Windows > система.**</span><span class="sxs-lookup"><span data-stu-id="fecc5-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="fecc5-121">В області праворуч перегляньте список униз  по стовпцях Джерело, доки не побачите події зі значенням Source **value MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="fecc5-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="fecc5-122">Виділіть кожну таку подію та перегляньте відомості про результат у полі на **вкладці** Загальні під списком.</span><span class="sxs-lookup"><span data-stu-id="fecc5-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
