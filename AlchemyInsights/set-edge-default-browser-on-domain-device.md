---
title: Установлення Microsoft Edge браузером за замовчуванням на пристрої, підключеному до домену
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491874"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="963ba-102">Установлення Microsoft Edge браузером за замовчуванням на пристрої, підключеному до домену</span><span class="sxs-lookup"><span data-stu-id="963ba-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="963ba-103">Установіть Microsoft Edge як стандартний браузер:</span><span class="sxs-lookup"><span data-stu-id="963ba-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="963ba-104">[Створіть файл конфігурації зв'язування за](https://go.microsoft.com/fwlink/?linkid=2132437) замовчуванням і зберігайте його локально або в мережевій спільній мережевій службі.</span><span class="sxs-lookup"><span data-stu-id="963ba-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="963ba-105">Відкрийте редактор групової політики, а потім перейдіть до статті Адміністративні шаблони конфігурації комп'ютера. Файловий  >    >  **провідник компонентів Windows.**  >  </span><span class="sxs-lookup"><span data-stu-id="963ba-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="963ba-106">Виберіть **елемент Установити файл конфігурації зв'язків за замовчуванням.**</span><span class="sxs-lookup"><span data-stu-id="963ba-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="963ba-107">Виберіть **Параметр політики**, а потім виберіть Увімкнуто . </span><span class="sxs-lookup"><span data-stu-id="963ba-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="963ba-108">У **розділі** Параметри введіть розташування файлу конфігурації зв'язку за замовчуванням, а потім натисніть кнопку **OK.**</span><span class="sxs-lookup"><span data-stu-id="963ba-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
