---
title: Виправлення неполадок синхронізації паролів
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387898"
---
# <a name="troubleshoot-password-synchronization"></a>Виправлення неполадок синхронізації паролів

Щоб вирішити проблеми з синхронізацією паролів, почніть з використання цього сад підключення виправлення неполадок завдання, щоб визначити, чому паролі не синхронізуються. Для початку перейдіть до [керування прямою синхронізацією](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Відкрийте новий сеанс Windows PowerShell на сервері Azure AD-підключення та виберіть параметр запуск із **правами адміністратора** .

2. Запустіть Set-виконання політики, Пульс, або набір-виконання політики необмежений.

3. Запустіть майстер Azure AD-підключення.

4. Перейдіть на сторінку додаткових завдань > **Виправлення неполадок**  >  **Далі**.

5. Виберіть **запустити** , щоб відкрити меню виправлення неполадок PowerShell.

6. Виберіть **Виправлення неполадок, синхронізація пароля**.

    Зазвичай, це не синхронізація пароля для певного облікового запису користувача.

    **Нотатки** Не вдається виконати синхронізацію паролів, якщо остання успішна синхронізація пароля була деякий час назад.

Щоб дізнатися більше про виправлення неполадок синхронізація пароля [, див.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)