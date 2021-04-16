---
title: Файл, відкритий лише для читання
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813205"
---
# <a name="file-open-read-only"></a><span data-ttu-id="d8f7d-102">Файл, відкритий лише для читання</span><span class="sxs-lookup"><span data-stu-id="d8f7d-102">File open read-only</span></span>

<span data-ttu-id="d8f7d-103">Під час відкриття файлів вони можуть відкриватись лише для читання.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="d8f7d-104">У деяких випадках це з міркуванням безпеки (наприклад, коли ви відкриваєте файли з Інтернету), а іноді це може бути через параметр, який можна змінити.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="d8f7d-105">Нижче наведено деякі сценарії, коли файл відкривається в режимі лише для читання, а також описано, як його змінити.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="d8f7d-106">**Антивірусна програма полягає в тому, що вони відкривають доступ лише для читання**</span><span class="sxs-lookup"><span data-stu-id="d8f7d-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="d8f7d-107">Деякі антивірусні програми можуть захистити вас від потенційно небезпечних файлів, відкривши їх лише для читання.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="d8f7d-108">Щоб дізнатися, як налаштувати ці параметри, можливо, знадобиться з'ясувати це у свого постачальника антивірусного програмного забезпечення.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="d8f7d-109">Наприклад, bitDefender містить вміст про додавання виключень програм тут: Додавання виключень програм або процесів у Центрі керування [Bitdefender.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="d8f7d-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="d8f7d-110">**Властивості файлу доступні лише для читання?**</span><span class="sxs-lookup"><span data-stu-id="d8f7d-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="d8f7d-111">Ви можете перевірити властивості файлу, клацнувши файл правою кнопкою миші та вибравши властивості.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="d8f7d-112">Якщо прапорець "Лише для читання" вибрано, зніміть його та натисніть кнопку OK.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="d8f7d-113">**Вміст у безпечному поданні**</span><span class="sxs-lookup"><span data-stu-id="d8f7d-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="d8f7d-114">Файли з Інтернету та інших потенційно небезпечних розташцій можуть містити віруси, хробаки та інші види зловмисних програм, які можуть завдати шкоди комп'ютеру.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="d8f7d-115">Це також часто з вкладеннями електронної пошти або файлами, які ви завантажили.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="d8f7d-116">Щоб захистити комп'ютер, файли з цих потенційно небезпечних розташцій відкриваються в безпечному поданні.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="d8f7d-117">У безпечному поданні ви можете читати файл і переглядати його вміст, зменшуючи ризики.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="d8f7d-118">Докладні відомості про безпечне подання та змінення параметрів див. в статті Що таке [безпечне подання?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="d8f7d-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="d8f7d-119">**OneDrive заповнено?**</span><span class="sxs-lookup"><span data-stu-id="d8f7d-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="d8f7d-120">Якщо файл зберігається у OneDrive і сховище OneDrive заповнено, зберегти документ не вдасться, доки не буде вільно вільного простору.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="d8f7d-121">Щоб перевірити вільне місце у OneDrive, клацніть піктограму OneDrive у центрі сповіщень і виберіть пункт Керування сховищем. Крім того, можна перейти на сайт , увійти та занотувати обсяг використаного простору в лівому нижньому куті [https://onedrive.live.com](https://onedrive.live.com) екрана.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="d8f7d-122">**Office активовано?**</span><span class="sxs-lookup"><span data-stu-id="d8f7d-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="d8f7d-123">Якщо Office не активовано або термін дії передплати завершиться, ви можете переключити режим обмеженої функціональності лише для читання.</span><span class="sxs-lookup"><span data-stu-id="d8f7d-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="d8f7d-124">Відомості про те, як активувати Office, див. в статті Помилки про "неліцензований продукт" і помилки [активації в Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="d8f7d-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="d8f7d-125">**Якщо нічого не видається...**</span><span class="sxs-lookup"><span data-stu-id="d8f7d-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="d8f7d-126">Спробуйте перезавантажити комп'ютер</span><span class="sxs-lookup"><span data-stu-id="d8f7d-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="d8f7d-127">Інсталяція оновлень Office</span><span class="sxs-lookup"><span data-stu-id="d8f7d-127">Install Office updates</span></span>
    
- <span data-ttu-id="d8f7d-128">Відновлення з мережі для пакета Office</span><span class="sxs-lookup"><span data-stu-id="d8f7d-128">Perform an Online repair of Office</span></span>
    

