---
title: Повторюваний запис пристрою на порталі
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814537"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="9c70e-102">Повторюваний запис пристрою на порталі</span><span class="sxs-lookup"><span data-stu-id="9c70e-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="9c70e-103">Якщо пристрій неналежно повідомляє сайту диспетчера конфігурацій стан спільного керування, на порталі може відображатися 2 записи пристрою.</span><span class="sxs-lookup"><span data-stu-id="9c70e-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="9c70e-104">Щоб перевірити стан спільної керування на пристрої, ознайомтеся зі стовпцем **Спільне керування** для пристрою в консолі диспетчера конфігурацій.</span><span class="sxs-lookup"><span data-stu-id="9c70e-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="9c70e-105">Якщо стовпець не відображається, його можна додати, клацнувши правою кнопкою миші будь-який заголовок стовпця та вибравши його зі списку.</span><span class="sxs-lookup"><span data-stu-id="9c70e-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="9c70e-106">Значення параметра "Спільне керування" має бути **Так**.</span><span class="sxs-lookup"><span data-stu-id="9c70e-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="9c70e-107">Якщо параметр має значення **Ні**, відкрийте аплет клієнта диспетчера конфігурацій на клієнтському пристрої та встановіть прапорець для властивості **Спільне керування** на вкладці "Загальне".</span><span class="sxs-lookup"><span data-stu-id="9c70e-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="9c70e-108">Якщо параметр має значення **Увімкнуто**, це вказує на проблеми з клієнтським зв’язком з точкою керування.</span><span class="sxs-lookup"><span data-stu-id="9c70e-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="9c70e-109">Ознайомтеся з **CcmMessaging. log** на пристрої, щоб дослідити потенційні проблеми з підключенням.</span><span class="sxs-lookup"><span data-stu-id="9c70e-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="9c70e-110">Якщо параметр має значення **Вимкнуто**, а пристрій зареєстровано в Inteune, переконайтеся, що цей пристрій одержав політику спільного керування, переглянувши **Comeanemempentandler.log** на пристрої.</span><span class="sxs-lookup"><span data-stu-id="9c70e-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
