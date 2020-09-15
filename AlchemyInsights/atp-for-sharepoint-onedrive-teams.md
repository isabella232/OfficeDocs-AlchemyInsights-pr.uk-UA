---
title: "\"АТФ для SharePoint\", \"OneDrive\" і груп Microsoft"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715582"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="841c5-102">"АТФ для SharePoint", "OneDrive" і груп Microsoft</span><span class="sxs-lookup"><span data-stu-id="841c5-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="841c5-103">Виконайте наведені нижче дії, щоб активувати розширений захист від загроз:</span><span class="sxs-lookup"><span data-stu-id="841c5-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="841c5-104">Перейдіть на сторінку [https://protection.office.com](https://protection.office.com) та увійдіть за допомогою облікового запису глобального адміністратора або адміністратора безпеки.</span><span class="sxs-lookup"><span data-stu-id="841c5-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="841c5-105">В області переходів ліворуч у розділі **керування загрозою**виберіть команду **Policy** \> **надійні вкладення**політики.</span><span class="sxs-lookup"><span data-stu-id="841c5-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="841c5-106">Виберіть **Увімкнути АТФ для SharePoint, OneDrive і команд Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="841c5-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="841c5-107">[Створіть політику оповіщення про дії,](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) щоб отримувати сповіщення, коли ми Виявляйте зловмисними файлами.</span><span class="sxs-lookup"><span data-stu-id="841c5-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="841c5-108">Щоб отримати докладні вказівки, ознайомтеся з цією [темою](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="841c5-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="841c5-109">**Примітка**: за конструкцією АТФ не перевіряє кожний файл у службі SharePoint Online, OneDrive для бізнесу або команд Microsoft.</span><span class="sxs-lookup"><span data-stu-id="841c5-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="841c5-110">Файли буде перевірено в асинхронному процесі, за допомогою якого ви надаєте спільний доступ до дій, гостьової діяльності та сигналів загрози для ідентифікації зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="841c5-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="841c5-111">Щоб отримати докладніші відомості, ознайомтеся з цією [темою](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="841c5-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
