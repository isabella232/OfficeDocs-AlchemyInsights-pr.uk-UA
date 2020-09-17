---
title: Відновлення PST-файлу Перед імпортуванням
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799117"
---
# <a name="repair-pst-file-before-importing"></a>Відновлення PST-файлу Перед імпортуванням

Перш ніж імпортувати PST-файл у програмі Outlook, переконайтеся, що файл не пошкоджено, відновивши файл:

1. Вийдіть із програми Outlook.

2. Знайти та запустити `Scanpst.exe` в папці програми Office (C:\Program Files (x86) \ Microsoft Office\roro\office \<Version\> або \Microsoft Files\Microsoft Office\roof\ Office \<Version\> ).

3. У **засобі відновлення папки "Вхідні" в Microsoft Outlook**натисніть кнопку **Огляд** , щоб знайти PST-файл (наприклад, у c: \ Users \ користувачі \\<ім'я користувача \> \Appdata\local\microsoft\outlook). Виберіть PST-файл, а потім натисніть кнопку **Відкрити**.

4. Натисніть кнопку **почати** , щоб почати сканування.

5. Якщо у файлі виявлено помилки, натисніть кнопку **відновити**, а потім натисніть кнопку **OK** після завершення відновлення.

6. Повторіть спробу імпортувати файл PST у програмі Outlook.

Докладні відомості наведено в статті [відновлення файлів даних Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) і [вирішення проблем з імпортом PST-файлу Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
