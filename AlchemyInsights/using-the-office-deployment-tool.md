---
title: За допомогою Office виконання засобу розгортання
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898671"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="cbb6f-102">За допомогою засобу розгортання Office (у форматі ODT)</span><span class="sxs-lookup"><span data-stu-id="cbb6f-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="cbb6f-p101">Ви використовуєте в офісі розгортання інструмент (у форматі ODT) розгортати Office 365 у версіях Office. Розгортання засобу Office (setup.exe) запустити з командного рядка і використовує XML-файлі конфігурації, щоб визначити, які параметри для застосування під час розгортання Office.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="cbb6f-105">Завантажити останню версію Office виконання засобу розгортання з [Центру завантажень Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="cbb6f-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="cbb6f-p102">За допомогою [Office на приладі (жовтень)](https://config.office.com) виберіть ваші уподобання розгортання і створити XML-файл конфігурації. Експортувати файл конфігурації і пок локально ж папку, де проживає на setup.exe.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="cbb6f-p103">**Примітка:** Зазвичай виникають проблеми через до неправильно налаштований інсталяції Office або malformatted конфігураційних файлів. Щоб уникнути таких проблем, рекомендовано використовувати Office приладі створити файл конфігурації. Ви також можете імпортувати наявні файли конфігурації в приладі Office.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="cbb6f-p104">Від підвищеної командного рядка перейдіть до розташування, де setup.exe проживає і запустити засіб розгортання офіс в режим завантаження і вказати щойно збережений файл конфігурації. У цьому прикладі файл конфігурації називається Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="cbb6f-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="cbb6f-113">Запуск засобу розгортання офіс в налаштування режиму та вкажіть відповідний файл конфігурації.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="cbb6f-114">**Примітка:** Ви повинні запустити цей крок з клієнтського комп'ютера, на якому потрібно інсталювати Office і дозвіл місцевого адміністратора на цьому комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="cbb6f-p105">Щоб дізнатися більше про інструментом Office розгортання для Office 365 ProPlus сценаріїв розгортання, переглянути [Огляд розгортання засобу Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Для більш докладної інформації про те, як використовувати засіб настройок Office переглянути [Огляд Office приладі](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="cbb6f-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

