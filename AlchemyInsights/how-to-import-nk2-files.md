---
title: інструкції з імпорту-NK2-Files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780080"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="ec10b-102">Імпорт файлів NK2</span><span class="sxs-lookup"><span data-stu-id="ec10b-102">How to import .nk2 files</span></span> 

<span data-ttu-id="ec10b-103">Під час першого запуску програми Microsoft Outlook 2013, Outlook 2016, Outlook 2019 або Outlook для Microsoft 365 уперше кеш-пам'ять (збережений у файлі */Profile*. NK2) імпортується в прихований текст у сховищі повідомлень за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="ec10b-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="ec10b-104">Щоб імпортувати файли NK2 у програму Outlook 2013, Outlook 2016, Outlook 2019 або Outlook для Microsoft 365, переконайтеся, що файл NK2 міститься в такій папці:%AppData%\microsoft\ Outlook</span><span class="sxs-lookup"><span data-stu-id="ec10b-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="ec10b-105">**Зверніть увагу**: файл NK2 має бути таким самим іменем, що й у поточному профілі Outlook 2013 або Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="ec10b-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="ec10b-106">За замовчуванням ім'я профілю – "Outlook".</span><span class="sxs-lookup"><span data-stu-id="ec10b-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="ec10b-107">Щоб перевірити ім'я профілю, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="ec10b-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="ec10b-108">Натисніть кнопку **Пуск**і виберіть пункт **панель керування**.</span><span class="sxs-lookup"><span data-stu-id="ec10b-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="ec10b-109">Двічі клацніть елемент **пошта**.</span><span class="sxs-lookup"><span data-stu-id="ec10b-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="ec10b-110">У діалоговому вікні Настроювання пошти натисніть кнопку **Показати профілі**.</span><span class="sxs-lookup"><span data-stu-id="ec10b-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="ec10b-111">Натисніть кнопку **запустити**  >  **Run**.</span><span class="sxs-lookup"><span data-stu-id="ec10b-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="ec10b-112">У полі **Відкрити** введіть *outlook.exe/importnk2*, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="ec10b-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="ec10b-113">Після імпорту файлу NK2 вміст файлу буде об'єднано в наявний кеш псевдоніма, який зберігатиметься в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="ec10b-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="ec10b-114">**Примітка**. NK2 файл перейменовується за допомогою розширення імені файлу під час наступного запуску програми Outlook 2013, Outlook 2016, Outlook 2019 або Outlook для Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ec10b-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="ec10b-115">Якщо потрібно повторно імпортувати файл NK2, спочатку видаліть розширення імені файлу.</span><span class="sxs-lookup"><span data-stu-id="ec10b-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="ec10b-116">Докладні відомості наведено в статті [Імпорт або копіювання списку автозаповнення на інший комп'ютер](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="ec10b-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>