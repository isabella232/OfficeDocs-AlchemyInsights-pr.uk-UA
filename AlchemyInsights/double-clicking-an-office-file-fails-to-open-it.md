---
title: Не вдається відкрити файл Office, двічі клацнувши його
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814826"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="dac80-102">Не вдається відкрити файл Office, двічі клацнувши його</span><span class="sxs-lookup"><span data-stu-id="dac80-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="dac80-103">Якщо двічі клацнути файл Office, може з'явитися відкрита програма, але сам файл не відкривається.</span><span class="sxs-lookup"><span data-stu-id="dac80-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="dac80-104">Або може з'явитися таке повідомлення про помилку: "Під час надсилання команди до програми сталася помилка".</span><span class="sxs-lookup"><span data-stu-id="dac80-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="dac80-105">Для цього існує багато причин, але нижче наведено два найпоширеніших рішення.</span><span class="sxs-lookup"><span data-stu-id="dac80-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="dac80-106">В Excel зніміть прапорець DDE.</span><span class="sxs-lookup"><span data-stu-id="dac80-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="dac80-107">Його можна знайти, створивши нову книгу та вибравши елементи Файл **> Параметри > Додатково**.</span><span class="sxs-lookup"><span data-stu-id="dac80-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="dac80-108">У розділі **Загальні** зніміть прапорець Ігнорувати **інші програми, у яких використовується динамічний обмін даними (DDE).**</span><span class="sxs-lookup"><span data-stu-id="dac80-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="dac80-109">Запустіть відновлення з мережі, щоб відновити настройки за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="dac80-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="dac80-110">Натисніть кнопку Пуск у Windows і знайдіть "Панель керування".</span><span class="sxs-lookup"><span data-stu-id="dac80-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="dac80-111">Відкрийте Панель **керування та** виберіть елементи Програми > Програми **та засоби**.</span><span class="sxs-lookup"><span data-stu-id="dac80-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="dac80-112">Потім клацніть правою кнопкою **миші Microsoft Office [версія]** та виберіть **змінити > відновлення з мережі.**</span><span class="sxs-lookup"><span data-stu-id="dac80-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="dac80-113">Якщо жоден із цих рішень не підійшов, докладніший список рішень можна знайти в статті служби підтримки. Не вдається відкрити файл Office, двічі клацнувши [його.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="dac80-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
