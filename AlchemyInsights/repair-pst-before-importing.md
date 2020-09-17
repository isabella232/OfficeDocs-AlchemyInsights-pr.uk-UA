---
title: Відновлення PST-файлу Перед імпортуванням
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799117"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="b53ac-102">Відновлення PST-файлу Перед імпортуванням</span><span class="sxs-lookup"><span data-stu-id="b53ac-102">Repair .pst file before importing</span></span>

<span data-ttu-id="b53ac-103">Перш ніж імпортувати PST-файл у програмі Outlook, переконайтеся, що файл не пошкоджено, відновивши файл:</span><span class="sxs-lookup"><span data-stu-id="b53ac-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="b53ac-104">Вийдіть із програми Outlook.</span><span class="sxs-lookup"><span data-stu-id="b53ac-104">Exit Outlook.</span></span>

2. <span data-ttu-id="b53ac-105">Знайти та запустити `Scanpst.exe` в папці програми Office (C:\Program Files (x86) \ Microsoft Office\roro\office \<Version\> або \Microsoft Files\Microsoft Office\roof\ Office \<Version\> ).</span><span class="sxs-lookup"><span data-stu-id="b53ac-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="b53ac-106">У **засобі відновлення папки "Вхідні" в Microsoft Outlook**натисніть кнопку **Огляд** , щоб знайти PST-файл (наприклад, у c: \ Users \ користувачі \\<ім'я користувача \> \Appdata\local\microsoft\outlook).</span><span class="sxs-lookup"><span data-stu-id="b53ac-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="b53ac-107">Виберіть PST-файл, а потім натисніть кнопку **Відкрити**.</span><span class="sxs-lookup"><span data-stu-id="b53ac-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="b53ac-108">Натисніть кнопку **почати** , щоб почати сканування.</span><span class="sxs-lookup"><span data-stu-id="b53ac-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="b53ac-109">Якщо у файлі виявлено помилки, натисніть кнопку **відновити**, а потім натисніть кнопку **OK** після завершення відновлення.</span><span class="sxs-lookup"><span data-stu-id="b53ac-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="b53ac-110">Повторіть спробу імпортувати файл PST у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="b53ac-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="b53ac-111">Докладні відомості наведено в статті [відновлення файлів даних Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) і [вирішення проблем з імпортом PST-файлу Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="b53ac-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
