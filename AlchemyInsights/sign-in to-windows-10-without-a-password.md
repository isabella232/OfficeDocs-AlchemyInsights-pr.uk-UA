---
title: Вхід у Windows 10 без використання пароля
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830567"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="e6afe-102">Вхід у Windows 10 без використання пароля</span><span class="sxs-lookup"><span data-stu-id="e6afe-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="e6afe-103">Щоб не вводити пароль під час запуску Windows, радимо скористатися одним із параметрів безпечного входу у Windows Hello, як-от PIN-код, розпізнавання обличчя або відбитки пальців, якщо вони доступні.</span><span class="sxs-lookup"><span data-stu-id="e6afe-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="e6afe-104">Якщо ви справді хочете вимкнути безпечний вхід, див. наведені нижче інструкції "Автоматичний вхід у Windows 10".</span><span class="sxs-lookup"><span data-stu-id="e6afe-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="e6afe-105">**Захист Windows Hello альтернативні пароля облікового запису**</span><span class="sxs-lookup"><span data-stu-id="e6afe-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="e6afe-106">Виберіть елементи **Настройки > Облікові > параметри входу** (або клацніть [тут).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="e6afe-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e6afe-107">З'являться доступні параметри входу.</span><span class="sxs-lookup"><span data-stu-id="e6afe-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="e6afe-108">Наприклад:</span><span class="sxs-lookup"><span data-stu-id="e6afe-108">For example:</span></span>

![Параметри входу.](media/sign-in-options.png)

<span data-ttu-id="e6afe-110">Виберіть один із параметрів, щоб настроїти його.</span><span class="sxs-lookup"><span data-stu-id="e6afe-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="e6afe-111">Під час наступного запуску або розблокування Windows можна буде використовувати новий параметр замість пароля.</span><span class="sxs-lookup"><span data-stu-id="e6afe-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="e6afe-112">**Автоматичний вхід у Windows 10**</span><span class="sxs-lookup"><span data-stu-id="e6afe-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="e6afe-113">**Примітка.** Автоматичний вхід зручний, але впроваджує загрозу безпеці, особливо якщо ПК доступний кільком користувачам.</span><span class="sxs-lookup"><span data-stu-id="e6afe-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="e6afe-114">Натисніть кнопку **Пуск** на панелі завдань.</span><span class="sxs-lookup"><span data-stu-id="e6afe-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="e6afe-115">Введіть **netplwiz і** натисніть клавішу Enter, щоб відкрити вікно "Облікові записи користувачів".</span><span class="sxs-lookup"><span data-stu-id="e6afe-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="e6afe-116">У **полі Облікові** записи користувачів виберіть обліковий запис, у який потрібно автоматично входити під час запуску Windows.</span><span class="sxs-lookup"><span data-stu-id="e6afe-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="e6afe-117">Зніміть прапорець "Користувачі повинні вводити ім'я користувача та пароль для використання цього комп'ютера".</span><span class="sxs-lookup"><span data-stu-id="e6afe-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Користувачі повинні ввести ім'я користувача та пароль.](media/users-must-enter-username.png)

5. <span data-ttu-id="e6afe-119">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="e6afe-119">Click **OK**.</span></span> <span data-ttu-id="e6afe-120">Вам буде запропоновано ввести та підтвердити пароль для вибраного облікового запису.</span><span class="sxs-lookup"><span data-stu-id="e6afe-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="e6afe-121">Натисніть **кнопку OK,** щоб завершити.</span><span class="sxs-lookup"><span data-stu-id="e6afe-121">Click **OK** to finish.</span></span> <span data-ttu-id="e6afe-122">Під час наступного запуску Windows 10 вона автоматично ввійме у вибраний обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="e6afe-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
