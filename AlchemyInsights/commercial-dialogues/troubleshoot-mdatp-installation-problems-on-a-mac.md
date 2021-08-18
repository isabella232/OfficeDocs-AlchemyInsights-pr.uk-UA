---
title: Усунення несправностей інсталяції MDATP на комп'ютері Mac
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091111"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Усунення несправностей інсталяції MDATP на комп'ютері Mac

Якщо інсталяція вручну завершиться **помилкою,** на сторінці Зведення майстра інсталяції вказуватиме таке повідомлення про помилку:

"Під час інсталяції сталася помилка. Інсталятор виявив помилку, через яку сталася помилка інсталяції. Зверніться по допомогу до виробника програмного забезпечення".

Для розгортань MDM на сторінці також відображається загальна помилка інсталяції.

Хоча для користувачів немає точних помилок, ми зберігаємо файл журналу з перебігом інсталяції, у **/Library/Logs/Microsoft/mdatp/install.log.** До цього файлу журналу додається кожен сеанс інсталяції. Щоб вивести лише останній сеанс інсталяції, `sed` використовуйте .

Докладні відомості див. в статті Виправлення неполадок інсталяції розширеного захисту від розширеного захисту від захисника [Microsoft для Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
