---
title: Файл відкрити лише для читання
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: 4c774864a03b7dbc099f64b7906fa4a0bc26c63c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525764"
---
# <a name="file-open-read-only"></a><span data-ttu-id="10b9d-102">Файл відкрити лише для читання</span><span class="sxs-lookup"><span data-stu-id="10b9d-102">File open read-only</span></span>

<span data-ttu-id="10b9d-103">Ви можете виявити, що, коли ви відкриваєте файли, вони відкрито лише для читання.</span><span class="sxs-lookup"><span data-stu-id="10b9d-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="10b9d-104">У деяких випадках це для додаткової безпеки, наприклад, коли ви відкриваєте файли з Інтернету а в інших випадках, це може бути пов'язано параметр, який можна змінити.</span><span class="sxs-lookup"><span data-stu-id="10b9d-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="10b9d-105">Ось деякі сценарії, де відкривається файл лише для читання та деякі кроки можна почати, щоб змінити цю ситуацію.</span><span class="sxs-lookup"><span data-stu-id="10b9d-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="10b9d-106">**Мій антивірус спричинили їх появу відкрити лише для читання**</span><span class="sxs-lookup"><span data-stu-id="10b9d-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="10b9d-107">Деякі антивірусні програми може захистити комп'ютер від потенційно небезпечних файлів, відкривши їх лише для читання.</span><span class="sxs-lookup"><span data-stu-id="10b9d-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="10b9d-108">Може знадобитися зверніться до постачальника антивірусного, щоб дізнатися, як настроїти ці параметри.</span><span class="sxs-lookup"><span data-stu-id="10b9d-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="10b9d-109">BitDefender, наприклад, має вміст на додавання винятків програми тут: [як додати застосунок або виключення процесу в Bitdefender диспетчерського центру](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="10b9d-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="10b9d-110">**Властивості файлу вибрано лише для читання?**</span><span class="sxs-lookup"><span data-stu-id="10b9d-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="10b9d-111">Властивості файлів можна перевірити, клацнувши правою кнопкою миші по файлу та обравши властивості.</span><span class="sxs-lookup"><span data-stu-id="10b9d-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="10b9d-112">Якщо установлено атрибут читання, зніміть його та натисніть кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="10b9d-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="10b9d-113">**Тобто у захищеному режимі**</span><span class="sxs-lookup"><span data-stu-id="10b9d-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="10b9d-114">Файли з Інтернету та з інших потенційно небезпечних місцях можуть містити віруси, хробаки або інші види зловмисного програмного забезпечення, які можуть завдати шкоди вашому комп'ютеру.</span><span class="sxs-lookup"><span data-stu-id="10b9d-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="10b9d-115">Це також трапляється у випадку з вкладень електронної пошти або файли, завантажені.</span><span class="sxs-lookup"><span data-stu-id="10b9d-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="10b9d-116">Щоб захистити комп ' ютер від ці потенційно небезпечного розташування відкривання у безпечному поданні.</span><span class="sxs-lookup"><span data-stu-id="10b9d-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="10b9d-117">За допомогою безпечному поданні, ви можете прочитати файл і побачити їх зміст при одночасному зниженні ризиків.</span><span class="sxs-lookup"><span data-stu-id="10b9d-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="10b9d-118">Більш докладну інформацію про перегляд захищений і як змінити настройки, перегляньте цю статтю: [що таке безпечному поданні?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="10b9d-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="10b9d-119">**Сповнена OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="10b9d-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="10b9d-120">Якщо файл зберігається на OneDrive і OneDrive простір зберігання заповнено, можна не вдалося зберегти документ, поки ви перебуваєте під відведеного місця.</span><span class="sxs-lookup"><span data-stu-id="10b9d-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="10b9d-121">Ви можете перевірити ваш вільного місця на OneDrive, натиснувши значок OneDrive в центрі сповіщень і вибравши керування сховищем, або ви можете піти в [http://onedrive.live.com](http://onedrive.live.com), увійдіть і зверніть увагу, обсяг використаного простору в нижньому лівому куті екрану.</span><span class="sxs-lookup"><span data-stu-id="10b9d-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="10b9d-122">**Служба активації?**</span><span class="sxs-lookup"><span data-stu-id="10b9d-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="10b9d-123">Office не активовано чи підписки минув, ви можете бути читання функціонально обмеженому режимі.</span><span class="sxs-lookup"><span data-stu-id="10b9d-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="10b9d-124">Відомості про те, як активувати Office див: [неліцензійне продукту й активації помилок у Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="10b9d-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="10b9d-125">**Якщо все інше не дасть результатів...**</span><span class="sxs-lookup"><span data-stu-id="10b9d-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="10b9d-126">Спробуйте перезавантажити комп'ютер</span><span class="sxs-lookup"><span data-stu-id="10b9d-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="10b9d-127">Інсталяція оновлень Office</span><span class="sxs-lookup"><span data-stu-id="10b9d-127">Install Office updates</span></span>
    
- <span data-ttu-id="10b9d-128">Виконувати онлайн ремонт офісу</span><span class="sxs-lookup"><span data-stu-id="10b9d-128">Perform an Online repair of Office</span></span>
    

