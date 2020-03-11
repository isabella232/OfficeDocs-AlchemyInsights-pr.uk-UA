---
title: Вхід у Windows 10 без використання пароля
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588301"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="b0116-102">Вхід у Windows 10 без використання пароля</span><span class="sxs-lookup"><span data-stu-id="b0116-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="b0116-103">Щоб уникнути введення пароля під час запуску Windows, рекомендовано використовувати один із параметрів безпечного входу Windows Hello, наприклад PIN-код, розпізнавання облич або відбиток пальця, якщо доступно.</span><span class="sxs-lookup"><span data-stu-id="b0116-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="b0116-104">Якщо ви дійсно бажаєте вимкнути Безпечний вхід, перегляньте інструкції "автоматично входити до Windows 10" нижче.</span><span class="sxs-lookup"><span data-stu-id="b0116-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="b0116-105">**Безпечні альтернативи Windows Hello для пароля облікового запису**</span><span class="sxs-lookup"><span data-stu-id="b0116-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="b0116-106">Перейдіть до **налаштувань > облікових записів > Параметри входу** (або натисніть [тут](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="b0116-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="b0116-107">Доступні Параметри входу будуть перераховані.</span><span class="sxs-lookup"><span data-stu-id="b0116-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="b0116-108">Наприклад,</span><span class="sxs-lookup"><span data-stu-id="b0116-108">For example:</span></span>

![Параметри входу.](media/sign-in-options.png)

<span data-ttu-id="b0116-110">Клацніть один із варіантів, щоб настроїти його.</span><span class="sxs-lookup"><span data-stu-id="b0116-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="b0116-111">Наступного разу, коли ви починаєте або розблоковуватиме Windows, ви зможете використовувати новий параметр замість пароля.</span><span class="sxs-lookup"><span data-stu-id="b0116-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="b0116-112">**Автоматичний вхід у Windows 10**</span><span class="sxs-lookup"><span data-stu-id="b0116-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="b0116-113">**Примітка**: автоматичний вхід зручний, але вводить загрозу безпеці, особливо якщо ваш комп'ютер доступний декількома користувачами.</span><span class="sxs-lookup"><span data-stu-id="b0116-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="b0116-114">Натисніть кнопку **Пуск** на панелі завдань.</span><span class="sxs-lookup"><span data-stu-id="b0116-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="b0116-115">Введіть **netplwiz** і натисніть клавішу ENTER, щоб відкрити вікно облікові записи користувачів.</span><span class="sxs-lookup"><span data-stu-id="b0116-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="b0116-116">У **облікових записах користувачів**виберіть обліковий запис, для якого потрібно автоматично ввійти під час запуску Windows.</span><span class="sxs-lookup"><span data-stu-id="b0116-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="b0116-117">Зніміть прапорець біля пункту "користувачі повинні ввести ім'я користувача та пароль для використання цього комп'ютера".</span><span class="sxs-lookup"><span data-stu-id="b0116-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Користувачі повинні ввести логін і пароль варіант.](media/users-must-enter-username.png)

5. <span data-ttu-id="b0116-119">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="b0116-119">Click **OK**.</span></span> <span data-ttu-id="b0116-120">Вам буде запропоновано ввести і підтвердити пароль для вибраного облікового запису.</span><span class="sxs-lookup"><span data-stu-id="b0116-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="b0116-121">Натисніть кнопку **ОК** , щоб завершити.</span><span class="sxs-lookup"><span data-stu-id="b0116-121">Click **OK** to finish.</span></span> <span data-ttu-id="b0116-122">Під час наступного запуску Windows 10 буде автоматично входити в вибраний обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="b0116-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
