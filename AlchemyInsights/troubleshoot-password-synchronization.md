---
title: Усунення несправностей із синхронізацією паролів
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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105799"
---
# <a name="troubleshoot-password-synchronization"></a>Усунення несправностей із синхронізацією паролів

Щоб усунути проблеми із синхронізацією паролів, розпочніть із цього завдання AAD Підключення щоб з'ясувати, чому паролі не синхронізуються. Щоб почати, перейдіть до керування [прямою синхронізацією.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Відкрийте новий сеанс Windows PowerShell на сервері Azure AD Підключення і виберіть **параметр У режимі** адміністратора.

2. Запустіть Set-ExecutionPolicy RemoteSigned або Set-ExecutionPolicy Unrestricted.

3. Запустіть майстер Підключення Azure AD.

4. Перейдіть на сторінку Додаткові завдання та виберіть > **Наступне**  >  **виправлення неполадок.**

5. Натисніть **кнопку Запустити,** щоб відкрити меню виправлення неполадок PowerShell.

6. Виберіть виправлення **неполадок із синхронізацією паролів**.

    Зазвичай проблема полягає в тому, що пароль не синхронізовано для певного облікового запису користувача.

    **Нотатки** Синхронізація паролів не завершиться, якщо час останньої успішної синхронізації паролів минуло.

Докладні відомості про виправлення неполадок із синхронізацією гешування паролів див. в Підключення [Azure AD.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)