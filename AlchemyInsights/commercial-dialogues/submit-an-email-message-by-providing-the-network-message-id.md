---
title: Надсилання повідомлення електронної пошти шляхом надання ІДЕНТИФІКАТОРА мережного повідомлення
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748204"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="27990-102">Надсилання повідомлення електронної пошти шляхом надання ІДЕНТИФІКАТОРА мережного повідомлення</span><span class="sxs-lookup"><span data-stu-id="27990-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="27990-103">У **поданні "Нове подання** " виберіть пункт **Електронна пошта** та **ідентифікатор мережного повідомлення**.</span><span class="sxs-lookup"><span data-stu-id="27990-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="27990-104">Виконайте наведені нижче дії, щоб отримати код повідомлення для повідомлення електронної пошти в програмі Outlook:</span><span class="sxs-lookup"><span data-stu-id="27990-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="27990-105">Двічі клацніть повідомлення електронної пошти, щоб відкрити його.</span><span class="sxs-lookup"><span data-stu-id="27990-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="27990-106">Виберіть пункт  >  **Властивості** файлу.</span><span class="sxs-lookup"><span data-stu-id="27990-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="27990-107">Відкрийте блокнот або пустий документ Word, а потім скопіюйте та вставте вміст, знайдений у полі **заголовки в Інтернеті** , у відкритий документ для кращої видимості.</span><span class="sxs-lookup"><span data-stu-id="27990-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="27990-108">Знайдіть поле **X-MS-Exchange-організація-мережа-повідомлення-ідентифікатор** поля.</span><span class="sxs-lookup"><span data-stu-id="27990-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="27990-109">Значення після **:** ідентифікатор, необхідний для надсилання.</span><span class="sxs-lookup"><span data-stu-id="27990-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="27990-110">У розділі **одержувачі**, якщо повідомлення електронної пошти, що приземлився в папці "Небажана пошта" для всіх одержувачів цього повідомлення електронної пошти, натисніть **кнопку "Виділити все**".</span><span class="sxs-lookup"><span data-stu-id="27990-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="27990-111">Якщо ні, виберіть лише користувач, який повідомив про цю проблему.</span><span class="sxs-lookup"><span data-stu-id="27990-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="27990-112">У розділі **причина для надсилання**, якщо вибрати елемент **має бути заблоковано**, укажіть, чи потрібно, щоб повідомлення було заблоковано **як спам**, **фішинг** або **зловмисне програмне забезпечення**, а потім натисніть кнопку **Надіслати**.</span><span class="sxs-lookup"><span data-stu-id="27990-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="27990-113">Щоб отримати докладні відомості, Дізнайтеся, [як надіслати підозрілого спаму, phpish, URL-адреси та файли до корпорації Майкрософт для сканування](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="27990-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
