---
title: Використання засобу розгортання Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726269"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="3d550-102">Використання засобу розгортання Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="3d550-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="3d550-103">Для розгортання Office 365 версії Office використовується засіб розгортання Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="3d550-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="3d550-104">Засіб розгортання Office (Setup. exe) запускається з командного рядка та використовує XML-файл конфігурації, щоб визначити, які параметри застосовувати під час розгортання Office.</span><span class="sxs-lookup"><span data-stu-id="3d550-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="3d550-105">Завантажити останню версію засобу розгортання Office, з [центру завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="3d550-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="3d550-106">Скористайтеся [засобом настроювання Office (Oct)](https://config.office.com) , щоб вибрати параметри розгортання та створити XML-файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="3d550-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="3d550-107">Експортуйте конфігураційний файл і розмістіть його локально в тій самій теці, де знаходиться програма Setup. exe.</span><span class="sxs-lookup"><span data-stu-id="3d550-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="3d550-108">**Примітка:** Проблеми з інсталяцією Office зазвичай виникають через неправильно налаштовані або неформатовані файли конфігурації.</span><span class="sxs-lookup"><span data-stu-id="3d550-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="3d550-109">Щоб уникнути таких проблем, рекомендовано використовувати засіб настроювання Office для створення файлу конфігурації.</span><span class="sxs-lookup"><span data-stu-id="3d550-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="3d550-110">Ви також можете імпортувати наявні файли конфігурації в засіб настроювання Office.</span><span class="sxs-lookup"><span data-stu-id="3d550-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="3d550-111">У командному рядку в режимі адміністратора перейдіть до розташування, де Setup. exe розміщено та запустіть засіб розгортання Office у режим завантаження та вкажіть щойно збережений файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="3d550-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="3d550-112">У цьому прикладі файл конфігурації має ім'я конфігурації. XML:</span><span class="sxs-lookup"><span data-stu-id="3d550-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="3d550-113">Запустіть засіб розгортання Office, у режимі настроювання та вкажіть файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="3d550-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="3d550-114">**Примітка:** Цей крок слід запускати з клієнтського комп'ютера, на якому потрібно інсталювати Office, і потрібно мати дозволи локального адміністратора на цьому комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="3d550-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="3d550-115">Щоб дізнатися більше про використання засобу розгортання Office для програм Microsoft 365 для сценаріїв корпоративного розгортання, перегляньте [Огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="3d550-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="3d550-116">Докладніші відомості про використання засобу настроювання Office наведено в [огляді засобу настроювання Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="3d550-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
