---
title: Виправлення неполадок із синхронізацією паролів
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664947"
---
# <a name="troubleshoot-password-synchronization"></a>Виправлення неполадок із синхронізацією паролів

Щоб усунути проблеми з синхронізацією паролів, запустіть цей параметр, щоб визначити, чому паролі не синхронізуються. Щоб почати, перейдіть на сторінку [керування прямим синхронізацією](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Відкрийте новий сеанс Windows PowerShell на веб-сервері Azure AD Connect і виберіть параметр " **Запуск із правами адміністратора** ".

2. Виконати віддалено або політику настроювання політики настроювання, не обмежено.

3. Запустіть майстер підключення до Azure AD Connect.

4. Перейдіть на сторінку додаткові завдання, > **виправити неполадку**  >  **Далі**.

5. Натисніть кнопку **Запуск** , щоб відкрити меню виправлення неполадок PowerShell.

6. Виберіть пункт **виправляти неполадки синхронізації пароля**.

    Ця проблема зазвичай не синхронізується з певним обліковим записом користувача.

    **Нотатки** Синхронізація пароля не вдалася, якщо останнє успішне синхронізації пароля було якийсь час назад.

Докладні відомості про виправлення неполадок із синхронізацією паролів наведено в статті [Виправлення неполадок із синхронізацією гешування паролів за допомогою синхронізації Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).