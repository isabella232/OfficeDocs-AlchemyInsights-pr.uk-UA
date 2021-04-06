---
title: Інсталяція Office і OneDrive на віртуальному робочому столі Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596029"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Інсталяція Office і OneDrive на віртуальному робочому столі Windows

1. [Підготуйте та налаштуйте зразок зображення VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Створіть віртуальну машину (VM), якщо її ще не створено.

1. [Інсталюйте пакет Office у режимі активації на спільному комп'ютері.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Активація на спільному комп'ютері дає змогу кільком користувачам отримувати доступ до Office.

1. [Інсталюйте OneDrive у режимі на комп'ютері.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Зазвичай програму OneDrive інстальовано для кожного користувача, але тут її потрібно інсталювати на комп'ютер.