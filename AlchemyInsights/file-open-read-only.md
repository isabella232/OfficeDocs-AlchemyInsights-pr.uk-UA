---
title: Відкриття файлу лише для читання
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745628"
---
# <a name="file-open-read-only"></a><span data-ttu-id="a3ebf-102">Відкриття файлу лише для читання</span><span class="sxs-lookup"><span data-stu-id="a3ebf-102">File open read-only</span></span>

<span data-ttu-id="a3ebf-103">Ви можете виявити, що коли ви відкриваєте файли, вони відкриваються лише для читання.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="a3ebf-104">У деяких випадках це – додаткова безпека, наприклад, коли ви відкриваєте файли з Інтернету та інші часи, це може бути пов'язано з параметром, який можна змінити.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="a3ebf-105">Нижче наведено кілька сценаріїв, у яких файл відкривається лише для читання, а також можливі кроки, які можна змінити.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="a3ebf-106">**Мій антивірус примушуючи їх відкрити лише для читання**</span><span class="sxs-lookup"><span data-stu-id="a3ebf-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="a3ebf-107">Деякі антивірусні програми можуть захистити вас від потенційно небезпечних файлів, відкривши їх лише для читання.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="a3ebf-108">Щоб дізнатися, як налаштувати ці параметри, може знадобитися звернутися до свого постачальника антивірусного програмного забезпечення.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="a3ebf-109">BitDefender, наприклад, має вміст для додавання виключень програм тут: [як додати виключення програм або процесів у центрі керування BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="a3ebf-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="a3ebf-110">**Чи настроєно властивості файлу лише для читання?**</span><span class="sxs-lookup"><span data-stu-id="a3ebf-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="a3ebf-111">Ви можете перевірити властивості файлу, клацнувши його правою кнопкою миші та вибравши пункт Властивості.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="a3ebf-112">Якщо встановлено атрибут "лише для читання", його можна зняти, а потім натисніть кнопку OK.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="a3ebf-113">**Вміст перебуває в безпечному поданні**</span><span class="sxs-lookup"><span data-stu-id="a3ebf-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="a3ebf-114">Файли з Інтернету та інших потенційно небезпечних розташувань можуть містити віруси, хробаки та інші види зловмисних програм, які можуть зашкодити комп'ютеру.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="a3ebf-115">Це також зазвичай стосується вкладень електронної пошти або файлів, які ви завантажили.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="a3ebf-116">Щоб захистити комп'ютер, файли з цих потенційно небезпечних розташувань відкриваються в безпечному поданні.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="a3ebf-117">За допомогою захищеного подання можна прочитати файл і побачити його вміст, зменшивши ризики.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="a3ebf-118">Докладні відомості про захищене подання та способи змінення настройок наведено в цій статті: що таке [захищене подання?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="a3ebf-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="a3ebf-119">**Чи заповнено її повними?**</span><span class="sxs-lookup"><span data-stu-id="a3ebf-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="a3ebf-120">Якщо файл зберігається в службі OneDrive, а обсяг сховища OneDrive заповнено, ви не зможете зберегти документ, доки не буде виділено простір.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="a3ebf-121">Ви можете перевірити вільний простір у службі "OneDrive", клацнувши піктограму OneDrive в центрі сповіщень і вибравши елемент керування сховищем, або ж ви можете перейти до [https://onedrive.live.com](https://onedrive.live.com) входу, ввійти та занотуйте обсяг використаного простору в нижньому лівому куті екрана.</span><span class="sxs-lookup"><span data-stu-id="a3ebf-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="a3ebf-122">**Чи активовано Office?**</span><span class="sxs-lookup"><span data-stu-id="a3ebf-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="a3ebf-123">Якщо Office не активовано або термін дії вашої передплатою минув, можливо, ви могли бути в режимі "лише для читання".</span><span class="sxs-lookup"><span data-stu-id="a3ebf-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="a3ebf-124">Щоб отримати відомості про активацію Office, див.: [неліцензований продукт і помилки активації в Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="a3ebf-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="a3ebf-125">**Якщо нічого не допомагає...**</span><span class="sxs-lookup"><span data-stu-id="a3ebf-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="a3ebf-126">Спроба перезавантажити комп'ютер</span><span class="sxs-lookup"><span data-stu-id="a3ebf-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="a3ebf-127">Інсталяція оновлень Office</span><span class="sxs-lookup"><span data-stu-id="a3ebf-127">Install Office updates</span></span>
    
- <span data-ttu-id="a3ebf-128">Виконання онлайнового відновлення Office</span><span class="sxs-lookup"><span data-stu-id="a3ebf-128">Perform an Online repair of Office</span></span>
    

