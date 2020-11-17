---
title: Використання засобу розгортання Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085853"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="80a71-102">Використання засобу розгортання Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="80a71-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="80a71-103">Ви використовуєте засіб розгортання Office (ODT), щоб розгорнути версії Office 365.</span><span class="sxs-lookup"><span data-stu-id="80a71-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="80a71-104">Засіб розгортання Office (setupodt.exe) запускається з командного рядка та використовує XML-файл конфігурації, щоб визначити, які настройки слід застосувати під час розгортання Office.</span><span class="sxs-lookup"><span data-stu-id="80a71-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="80a71-105">Завантажте найновішу версію засобу розгортання Office в [центрі завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="80a71-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="80a71-106">Скористайтеся [засобом настроювання Office (жовтень)](https://config.office.com) , щоб вибрати параметри розгортання та створити XML-файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="80a71-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="80a71-107">Експортуйте файл конфігурації та розмістіть його локально в тій самій папці, де знаходиться setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="80a71-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="80a71-108">**Примітка.** Проблеми з інсталяцією Office зазвичай виникають через неправильне настроювання або файли конфігураційних файлів.</span><span class="sxs-lookup"><span data-stu-id="80a71-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="80a71-109">Щоб уникнути таких проблем, радимо використовувати засіб настроювання Office, щоб створити файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="80a71-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="80a71-110">Ви також можете імпортувати доступні файли конфігурації до засобу настроювання Office.</span><span class="sxs-lookup"><span data-stu-id="80a71-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="80a71-111">У командному рядку зі підвищеними параметрами перейдіть до розташування, у якому setupodt.exe розташовано та запустіть засіб розгортання Office у режимі завантаження та вкажіть щойно збережений файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="80a71-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="80a71-112">У цьому прикладі файл конфігурації має назву Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="80a71-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="80a71-113">4. запустіть засіб розгортання Office у режимі настроювання та вкажіть файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="80a71-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="80a71-114">**Примітка.** Потрібно виконати цей крок із клієнтського комп'ютера, на якому потрібно інсталювати Office, і на цьому комп'ютері потрібно мати дозволи локального адміністратора.</span><span class="sxs-lookup"><span data-stu-id="80a71-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="80a71-115">Щоб дізнатися більше про використання засобу розгортання Office для програм Microsoft 365 для сценаріїв розгортання підприємств, ознайомтеся [зі статтею огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="80a71-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="80a71-116">Докладні відомості про використання засобу настроювання Office наведено в розділі [Огляд засобу настроювання Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="80a71-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
