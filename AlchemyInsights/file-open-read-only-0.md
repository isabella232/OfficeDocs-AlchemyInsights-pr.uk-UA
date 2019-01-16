---
title: Файл відкрити лише для читання
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: cbc3a97debc70ce7be02f651253c71651bbb2643
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318730"
---
# <a name="file-open-read-only"></a><span data-ttu-id="16426-102">Файл відкрити лише для читання</span><span class="sxs-lookup"><span data-stu-id="16426-102">File open read-only</span></span>

<span data-ttu-id="16426-p101">Ви можете виявити, що, коли ви відкриваєте файли, вони відкрито лише для читання. У деяких випадках це для додаткової безпеки, наприклад, коли ви відкриваєте файли з Інтернету а в інших випадках, це може бути пов'язано параметр, який можна змінити. Ось деякі сценарії, де відкривається файл лише для читання та деякі кроки можна почати, щоб змінити цю ситуацію.</span><span class="sxs-lookup"><span data-stu-id="16426-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="16426-106">**Мій антивірус спричинили їх появу відкрити лише для читання**</span><span class="sxs-lookup"><span data-stu-id="16426-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="16426-p102">Деякі антивірусні програми може захистити комп'ютер від потенційно небезпечних файлів, відкривши їх лише для читання. Може знадобитися зверніться до постачальника антивірусного, щоб дізнатися, як настроїти ці параметри. BitDefender, наприклад, має вміст на додавання винятків програми тут: [як додати застосунок або виключення процесу в Bitdefender диспетчерського центру](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="16426-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="16426-110">**Властивості файлу вибрано лише для читання?**</span><span class="sxs-lookup"><span data-stu-id="16426-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="16426-p103">Властивості файлів можна перевірити, клацнувши правою кнопкою миші по файлу та обравши властивості. Якщо установлено атрибут читання, зніміть його та натисніть кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="16426-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="16426-113">**Тобто у захищеному режимі**</span><span class="sxs-lookup"><span data-stu-id="16426-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="16426-p104">Файли з Інтернету та з інших потенційно небезпечних місцях можуть містити віруси, хробаки або інші види зловмисного програмного забезпечення, які можуть завдати шкоди вашому комп'ютеру. Це також трапляється у випадку з вкладень електронної пошти або файли, завантажені. Щоб захистити комп ' ютер від ці потенційно небезпечного розташування відкривання у безпечному поданні. За допомогою безпечному поданні, ви можете прочитати файл і побачити їх зміст при одночасному зниженні ризиків. Більш докладну інформацію про перегляд захищений і як змінити настройки, перегляньте цю статтю: [що таке безпечному поданні?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="16426-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="16426-119">**Сповнена OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="16426-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="16426-p105">Якщо файл зберігається на OneDrive і OneDrive простір зберігання заповнено, можна не вдалося зберегти документ, поки ви перебуваєте під відведеного місця. Ви можете перевірити ваш вільного місця на OneDrive, натиснувши значок OneDrive в центрі сповіщень і вибравши керування сховищем, або ви можете піти в [http://onedrive.live.com](http://onedrive.live.com), увійдіть і зверніть увагу, обсяг використаного простору в нижньому лівому куті екрану.</span><span class="sxs-lookup"><span data-stu-id="16426-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="16426-122">**Служба активації?**</span><span class="sxs-lookup"><span data-stu-id="16426-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="16426-p106">Office не активовано чи підписки минув, ви можете бути читання функціонально обмеженому режимі. Відомості про те, як активувати Office див: [неліцензійне продукту й активації помилок у Office](https://support.office.com/en-us/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="16426-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/en-us/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="16426-125">**Якщо все інше не дасть результатів...**</span><span class="sxs-lookup"><span data-stu-id="16426-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="16426-126">Спробуйте перезавантажити комп'ютер</span><span class="sxs-lookup"><span data-stu-id="16426-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="16426-127">Інсталяція оновлень Office</span><span class="sxs-lookup"><span data-stu-id="16426-127">Install Office updates</span></span>
    
- <span data-ttu-id="16426-128">Виконувати онлайн ремонт офісу</span><span class="sxs-lookup"><span data-stu-id="16426-128">Perform an Online repair of Office</span></span>
    

