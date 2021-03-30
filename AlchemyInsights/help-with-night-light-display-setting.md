---
title: Допоможіть настройка нічного світла
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405185"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="62bc6-102">Допоможіть настройка нічного світла</span><span class="sxs-lookup"><span data-stu-id="62bc6-102">Help with the night light display setting</span></span>

<span data-ttu-id="62bc6-103">Докладні відомості про параметри відображення вночі див. в розділі Налаштування [дисплея для використання вночі у Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="62bc6-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="62bc6-104">Якщо в розділі "Настройки" не відображаються параметри нічного світла, перевірте драйвер дисплея:</span><span class="sxs-lookup"><span data-stu-id="62bc6-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="62bc6-105">Клацніть поле пошуку на панелі завдань і введіть **Диспетчер** пристроїв , а потім виберіть пункт **Диспетчер пристроїв** у результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="62bc6-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="62bc6-106">**Розгорніть розділ Відеоадаптери**.</span><span class="sxs-lookup"><span data-stu-id="62bc6-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="62bc6-107">На жаль, функція нічнику недоступна, якщо пристрій використовує драйвер DisplayLink або драйвер Basic Display.</span><span class="sxs-lookup"><span data-stu-id="62bc6-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="62bc6-108">Функція нічного світла використовує нещодавню графічну технологію, тому може знадобитися оновити драйвер дисплея:</span><span class="sxs-lookup"><span data-stu-id="62bc6-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="62bc6-109">Щоб перевірити наявність оновлень, виберіть **Пуск**  >  **оновлення**  >  **параметрів & Windows**  >  **Update** Перевірити  >  **наявність оновлень.**</span><span class="sxs-lookup"><span data-stu-id="62bc6-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="62bc6-110">АБО</span><span class="sxs-lookup"><span data-stu-id="62bc6-110">OR</span></span>

- <span data-ttu-id="62bc6-111">Відвідайте веб-сайт служби підтримки виробника обладнання, щоб вручну завантажити та інсталювати найновіші драйвери дисплея.</span><span class="sxs-lookup"><span data-stu-id="62bc6-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="62bc6-112">Скидання нічного світла в реєстрі</span><span class="sxs-lookup"><span data-stu-id="62bc6-112">Reset night light in the registry</span></span>

<span data-ttu-id="62bc6-113">Якщо не вдалося оновити драйвер дисплея, можливо, знадобиться скинути нічне світло в реєстрі.</span><span class="sxs-lookup"><span data-stu-id="62bc6-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="62bc6-114">**Застереження.** Цей крок виправлення неполадок рекомендовано тільки для досвідчених користувачів.</span><span class="sxs-lookup"><span data-stu-id="62bc6-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="62bc6-115">У разі внесення неправильних змін до реєстру можуть виникнути серйозні проблеми.</span><span class="sxs-lookup"><span data-stu-id="62bc6-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="62bc6-116">Для додаткового захисту, перед внесенням змін резервної копії реєстру, щоб можна було відновити його в разі виникнення проблем.</span><span class="sxs-lookup"><span data-stu-id="62bc6-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="62bc6-117">У полі пошуку введіть **regedit**, а потім виберіть **Пункт Редактор реєстру** в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="62bc6-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="62bc6-118">Перейдіть до такого розділу реєстру:</span><span class="sxs-lookup"><span data-stu-id="62bc6-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="62bc6-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="62bc6-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="62bc6-120">Експорт, а потім – наведений нижче підрозділ:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="62bc6-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="62bc6-121">Експорт, а потім видаліть такий підрозділ:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="62bc6-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="62bc6-122">Перезавантажте Windows і перевірте, чи доступні параметри нічного світла.</span><span class="sxs-lookup"><span data-stu-id="62bc6-122">Restart Windows and verify if the night light options are available.</span></span>


