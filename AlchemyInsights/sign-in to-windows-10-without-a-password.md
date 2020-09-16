---
title: Вхід у Windows 10 без використання пароля
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719974"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="f7efc-102">Вхід у Windows 10 без використання пароля</span><span class="sxs-lookup"><span data-stu-id="f7efc-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="f7efc-103">Щоб не вводити пароль під час запуску Windows, радимо використовувати один із безпечних параметрів входу Windows, наприклад PIN-код, розпізнавання облич або відбитки пальців, якщо доступно.</span><span class="sxs-lookup"><span data-stu-id="f7efc-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="f7efc-104">Якщо ви дійсно хочете вимкнути безпечну реєстрацію, ознайомтеся з наведеними нижче вказівками "автоматично входити в Windows 10".</span><span class="sxs-lookup"><span data-stu-id="f7efc-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="f7efc-105">**Захист облікового запису "Привіт" для Windows**</span><span class="sxs-lookup"><span data-stu-id="f7efc-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="f7efc-106">Послідовно виберіть елементи **настройки > облікові записи > Параметри входу** (або клацніть [тут](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="f7efc-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f7efc-107">Доступні варіанти входу буде наведено в списку.</span><span class="sxs-lookup"><span data-stu-id="f7efc-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="f7efc-108">Наприклад,</span><span class="sxs-lookup"><span data-stu-id="f7efc-108">For example:</span></span>

![Варіанти входу.](media/sign-in-options.png)

<span data-ttu-id="f7efc-110">Клацніть або торкніться одного з параметрів, щоб настроїти його.</span><span class="sxs-lookup"><span data-stu-id="f7efc-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="f7efc-111">Під час наступного запуску або розблокування Windows ви зможете використовувати новий параметр замість пароля.</span><span class="sxs-lookup"><span data-stu-id="f7efc-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="f7efc-112">**Автоматичне входу в ОС Windows 10**</span><span class="sxs-lookup"><span data-stu-id="f7efc-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="f7efc-113">**Примітка**: функція автоматичного входу зручна, але вона вводить ризик для безпеки, особливо якщо комп'ютер доступний для кількох користувачів.</span><span class="sxs-lookup"><span data-stu-id="f7efc-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="f7efc-114">Клацніть або торкніться кнопки **Пуск** на панелі завдань.</span><span class="sxs-lookup"><span data-stu-id="f7efc-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="f7efc-115">Введіть **netplwiz** і натисніть клавішу "ввести", щоб відкрити вікно "облікові записи користувачів".</span><span class="sxs-lookup"><span data-stu-id="f7efc-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="f7efc-116">У розділі **облікові записи користувачів**виберіть обліковий запис, який потрібно автоматично ввійти під час завантаження Windows.</span><span class="sxs-lookup"><span data-stu-id="f7efc-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="f7efc-117">Зніміть прапорець "користувачі мають ввести ім'я користувача та пароль, щоб використовувати цей комп'ютер".</span><span class="sxs-lookup"><span data-stu-id="f7efc-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Користувачі мають ввести ім'я користувача та пароль.](media/users-must-enter-username.png)

5. <span data-ttu-id="f7efc-119">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="f7efc-119">Click **OK**.</span></span> <span data-ttu-id="f7efc-120">З'явиться запит на введення та підтвердження пароля для вибраного облікового запису.</span><span class="sxs-lookup"><span data-stu-id="f7efc-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="f7efc-121">Натисніть кнопку **OK** , щоб завершити.</span><span class="sxs-lookup"><span data-stu-id="f7efc-121">Click **OK** to finish.</span></span> <span data-ttu-id="f7efc-122">Під час наступного завантаження Windows 10 буде автоматично входити в вибраний обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="f7efc-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
