---
title: Відмовлено в доступі під час зіставлення диска з SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668764"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="94353-102">Вирішення проблем із бібліотеками SharePoint, зіставленими з мережними дисками</span><span class="sxs-lookup"><span data-stu-id="94353-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="94353-103">Під час переходу на зіставлений мережний диск може з'явитися одне з таких повідомлень:</span><span class="sxs-lookup"><span data-stu-id="94353-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="94353-104">**\\Шлях не доступний. Можливо, у вас немає дозволу на використання цього мережевого ресурсу. Зверніться до адміністратора цього сервера, щоб дізнатися, чи є у вас дозволи на доступ.**</span><span class="sxs-lookup"><span data-stu-id="94353-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="94353-105">**Відмовлено в доступі. Перш ніж відкривати файли в цьому розташуванні, потрібно спочатку додати веб-сайт до списку надійних сайтів, перейти до веб-сайту та вибрати параметр для автоматичного входу.**</span><span class="sxs-lookup"><span data-stu-id="94353-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="94353-106">[Отримайте довідку з виправлення неполадок із зіставленими мережевими дисками](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="94353-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="94353-107">Зіставлення бібліотеки як мережевого диска тимчасовий і підтримується лише в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="94353-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="94353-108">Натомість [Синхронізуйте файли SharePoint за допомогою нового клієнта синхронізації "OneDrive"](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , яка містить [файли на вимогу](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="94353-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="94353-109">Доступ до всіх файлів у службі OneDrive без використання локального простору для сховища.</span><span class="sxs-lookup"><span data-stu-id="94353-109">Access all your files in OneDrive without using local storage space.</span></span>
  