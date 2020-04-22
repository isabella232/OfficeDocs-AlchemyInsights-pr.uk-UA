---
title: Файл відкрити лише для читання
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702795"
---
# <a name="file-open-read-only"></a><span data-ttu-id="ce6a5-102">Файл відкрити лише для читання</span><span class="sxs-lookup"><span data-stu-id="ce6a5-102">File open read-only</span></span>

<span data-ttu-id="ce6a5-103">Ви можете виявити, що під час відкриття файлів вони відкриваються лише для читання.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="ce6a5-104">У деяких випадках це для додаткової безпеки, наприклад, коли ви відкриваєте файли з Інтернету, і в інший час, це може бути пов'язано з настройці, які можуть бути змінені.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="ce6a5-105">Нижче наведено кілька сценаріїв, у яких файл відкривається лише для читання, а деякі кроки можна зробити для зміни.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="ce6a5-106">**Мій антивірус викликає їх відкрити тільки для читання**</span><span class="sxs-lookup"><span data-stu-id="ce6a5-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="ce6a5-107">Деякі антивірусні програми можуть захистити вас від потенційно небезпечних файлів, відкривши їх лише для читання.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="ce6a5-108">Щоб дізнатися, як налаштувати ці параметри, може знадобитися перевірити його у постачальника антивірусної програми.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="ce6a5-109">BitDefender, наприклад, має вміст на додавання виключень додатків тут: [як додати програму або виключення процесів у центр керування BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="ce6a5-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="ce6a5-110">**Чи встановлено властивості файлу лише для читання?**</span><span class="sxs-lookup"><span data-stu-id="ce6a5-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="ce6a5-111">Ви можете перевірити властивості файлу, клацнувши правою кнопкою миші на файлі і вибравши властивості.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="ce6a5-112">Якщо встановлено атрибут "тільки читання", його можна зняти та клацнути OK.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="ce6a5-113">**Вміст у захищеному поданні**</span><span class="sxs-lookup"><span data-stu-id="ce6a5-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="ce6a5-114">Файли з Інтернету та з інших потенційно небезпечних розташувань можуть містити віруси, хробаки або інші зловмисні програми, які можуть зашкодити комп'ютеру.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="ce6a5-115">Це також зазвичай стосується вкладень електронної пошти або файлів, які ви завантажили.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="ce6a5-116">Для захисту комп'ютера файли з цих потенційно небезпечних розташувань відкриваються в захищеному поданні.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="ce6a5-117">За допомогою безпечного подання можна прочитати файл і побачити його вміст під час зменшення ризиків.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="ce6a5-118">Щоб отримати додаткові відомості про захищений перегляд і як змінити настройки, див у цій статті: [що таке захищений перегляд?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="ce6a5-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="ce6a5-119">**Є OneDrive повний?**</span><span class="sxs-lookup"><span data-stu-id="ce6a5-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="ce6a5-120">Якщо файл зберігається в OneDrive і ваш простір зберігання OneDrive заповнено, ви не зможете зберегти документ, доки ви не перебуваєте під відведеним простором.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="ce6a5-121">Ви можете перевірити свій вільний простір у OneDrive, натиснувши значок OneDrive в центрі сповіщень і вибравши керування сховищем, або ви можете перейти до [https://onedrive.live.com](https://onedrive.live.com), ввійти в систему та відзначити обсяг використовуваного простору в нижньому лівому на екрані.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="ce6a5-122">**Чи активовано Office?**</span><span class="sxs-lookup"><span data-stu-id="ce6a5-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="ce6a5-123">Якщо Office не активовано, або якщо термін дії передплати минув, можливо, ви могли б перебувати у режимі обмеженої функціональності лише для читання.</span><span class="sxs-lookup"><span data-stu-id="ce6a5-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="ce6a5-124">Відомості про те, як активувати Office див.: [ліцензовано продукту та помилки активації в Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="ce6a5-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="ce6a5-125">**Якщо все інше не вдається...**</span><span class="sxs-lookup"><span data-stu-id="ce6a5-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="ce6a5-126">Спробуйте перезапустити комп'ютер</span><span class="sxs-lookup"><span data-stu-id="ce6a5-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="ce6a5-127">Інсталяція оновлень Office</span><span class="sxs-lookup"><span data-stu-id="ce6a5-127">Install Office updates</span></span>
    
- <span data-ttu-id="ce6a5-128">Виконання онлайн відновлення Office</span><span class="sxs-lookup"><span data-stu-id="ce6a5-128">Perform an Online repair of Office</span></span>
    

