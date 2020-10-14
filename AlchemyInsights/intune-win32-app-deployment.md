---
title: Розгортання програм Win32 (inune)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461997"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="2d694-102">Розгортання програм Win32 (inune)</span><span class="sxs-lookup"><span data-stu-id="2d694-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="2d694-103">Microsoft Inune дає змогу використовувати Win32-програми, зокрема, але не обмежуються MSI і. Програма EXE для розгортання пристроїв із Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2d694-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="2d694-104">Використовуваний механізм розгортання вимагає, щоб на цільовому пристрої було представлено розширення керування Inune (IME).</span><span class="sxs-lookup"><span data-stu-id="2d694-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="2d694-105">Редактор IME буде автоматично інстальовано в результаті орієнтації на сценарій PowerShell або розгортання програм Win32 для користувача або пристрою.</span><span class="sxs-lookup"><span data-stu-id="2d694-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="2d694-106">Також є набір передумов, які потрібно виконати, щоб розгорнути програми Win32, які містять такі елементи:</span><span class="sxs-lookup"><span data-stu-id="2d694-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="2d694-107">Підтримувані платформи: операційна система Windows 10 версії 1607 або пізніша (корпоративні, Pro та навчальні версії).</span><span class="sxs-lookup"><span data-stu-id="2d694-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="2d694-108">Підтримується архітектура: x86 і x64.</span><span class="sxs-lookup"><span data-stu-id="2d694-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="2d694-109">Керування пристроями: під час приєднання до мережі та автоматичної реєстрації (включно з гібридним доменом, до якого приєдналися та групова політика, автоматично зараховані).</span><span class="sxs-lookup"><span data-stu-id="2d694-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="2d694-110">Формат пакетів програм:. файл **intunewin**  , підготовлений за допомогою [засобу підготовчої програми Win32 (Microsoft](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)).</span><span class="sxs-lookup"><span data-stu-id="2d694-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="2d694-111">Обмеження</span><span class="sxs-lookup"><span data-stu-id="2d694-111">Limitations:</span></span>
    - <span data-ttu-id="2d694-112">Максимальний розмір: 8GB.</span><span class="sxs-lookup"><span data-stu-id="2d694-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="2d694-113">Непідтримувана архітектура: озброєння.</span><span class="sxs-lookup"><span data-stu-id="2d694-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="2d694-114">Ознайомтеся з документами "[Додавання, призначення та відстеження програми Win32 в Microsoft InTune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" для інформації, пов'язаної з цими кроками.</span><span class="sxs-lookup"><span data-stu-id="2d694-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="2d694-115">Докладні відомості про виправлення неполадок розгортання програм у Windows, зокрема програми Win32, можна переглянути в наведених нижче документах.</span><span class="sxs-lookup"><span data-stu-id="2d694-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="2d694-116">Усунення проблем із інсталяцією програм</span><span class="sxs-lookup"><span data-stu-id="2d694-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="2d694-117">Виправлення неполадок із програмами Win32</span><span class="sxs-lookup"><span data-stu-id="2d694-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)