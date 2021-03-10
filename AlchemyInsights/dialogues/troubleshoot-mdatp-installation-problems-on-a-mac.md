---
title: Виправлення неполадок інсталяції MDATP на комп'ютері Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696100"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Виправлення неполадок інсталяції MDATP на комп'ютері Mac

Якщо не вдалося виконати інсталяцію вручну, на сторінці « **зведення** » майстра інсталяції відображається таке повідомлення про помилку:

"Під час інсталяції сталася помилка". Помилка інсталятора виявила помилку, яка призвела до помилки інсталяції. Зверніться до виробника програмного забезпечення, щоб отримати допомогу. "

У разі розгортання для MDM на сторінці відображається Загальна помилка інсталяції.

Хоча ми не відображаємо точні помилки для кінцевого користувача, ми зберігаємо файл журналу з прогресом інсталяції в **/Library/logs/Microsoft/mdatp/Install.log**. Кожний сеанс інсталяції додається до цього файлу журналу. Щоб вивести лише останній сеанс інсталяції, використовуйте її `sed` .

Докладні відомості наведено в статті [Виправлення неполадок із інсталяцією для системи захисту від захисника Microsoft для Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
