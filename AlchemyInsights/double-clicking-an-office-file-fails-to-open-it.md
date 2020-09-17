---
title: Не вдається відкрити файл Office двічі
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812100"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="2d084-102">Не вдається відкрити файл Office двічі</span><span class="sxs-lookup"><span data-stu-id="2d084-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="2d084-103">Після того як ви двічі клацаєте файл Office, ви можете побачити програму відкритою, але сам файл не відкривається.</span><span class="sxs-lookup"><span data-stu-id="2d084-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="2d084-104">Або може з'явитися повідомлення про помилку: "виникла помилка під час надсилання команди до програми".</span><span class="sxs-lookup"><span data-stu-id="2d084-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="2d084-105">Для цього є багато причин, але два найпоширеніші рішення:</span><span class="sxs-lookup"><span data-stu-id="2d084-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="2d084-106">У програмі Excel переконайтеся, що параметр DDE знято.</span><span class="sxs-lookup"><span data-stu-id="2d084-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="2d084-107">Цей параметр можна знайти, створивши нову книгу, а потім виберіть пункт **Параметри файлу > > додатково**.</span><span class="sxs-lookup"><span data-stu-id="2d084-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="2d084-108">У розділі **загальні** зніміть прапорець **Ігнорувати інші програми, які використовують динамічний обмін даними (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="2d084-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="2d084-109">Виконайте онлайнове відновлення, щоб відновити настройки за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="2d084-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="2d084-110">Натисніть кнопку Пуск Windows і знайдіть "панель керування".</span><span class="sxs-lookup"><span data-stu-id="2d084-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="2d084-111">Відкрийте **панель керування**та перейдіть до **програм > програм і функцій**.</span><span class="sxs-lookup"><span data-stu-id="2d084-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="2d084-112">Потім клацніть правою кнопкою миші пункт **Microsoft Office [версія]** і виберіть **змінити > онлайн-відновлення**.</span><span class="sxs-lookup"><span data-stu-id="2d084-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="2d084-113">Якщо жоден із цих рішень не працює, можна знайти повний список вирішень у статті підтримки, [двічі клацнувши файл Office, щоб відкрити його](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="2d084-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
