---
title: Приклад політики Microsoft Defender для безпечного вкладення в Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749192"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Приклад політики Microsoft Defender для безпечного вкладення в Office 365

Ці параметри дають змогу політиці під назвою " *без затримок* ", що доставляє повідомлення негайно, а потім повторно надає вкладення після того, як вони скануються:

- **Ім'я**: без затримок
- **Опис**: доставляє повідомлення негайно й повторно надає вкладення після сканування.
- **Відповідь**: виберіть параметр **динамічної доставки** . Докладні відомості наведено в статті [динамічна доставка в надійних політиці вкладень](https://go.microsoft.com/fwlink/?linkid=2092328).
- Розділ " **переспрямування вкладень** ": виберіть параметр, щоб **Увімкнути переспрямування**, а потім введіть адресу електронної пошти глобального адміністратора Microsoft 365, адміністратора системи безпеки або аналітика системи безпеки, які розслідуватимуть зловмисні вкладення.
- **Застосувати до** розділу: виберіть **домен одержувача**, а потім виберіть свій домен. Виберіть **Додати**, а потім натисніть **кнопку OK**. Завершивши, натисніть кнопку **зберегти**.

Щоб отримати докладні відомості, перегляньте елементи [надійні вкладення в програмі Microsoft Defender для Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
