---
title: Не вдається відкрити файл Office двічі клацнувши його
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965122"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Не вдається відкрити файл Office двічі клацнувши його

Якщо двічі клацнути Office, може з'явитися відкрита програма, але сам файл не відкривається. Або може з'явитися таке повідомлення про помилку: "Під час надсилання команди до програми сталася помилка". Для цього існує багато причин, але нижче наведено два найпоширеніших рішення.

- У Excel зніміть прапорець DDE. Його можна знайти, створивши нову книгу та вибравши елементи Файл **> Параметри > Додатково**. У розділі **Загальні** зніміть прапорець Ігнорувати інші програми, у яких використовуються **динамічні Exchange (DDE).**

- Запустіть відновлення з мережі, щоб відновити настройки за замовчуванням. Натисніть кнопку Windows Пуск" і знайдіть "Панель керування". Відкрийте Панель **керування та** виберіть елементи Програми > Програми **та засоби**. Потім клацніть правою кнопкою **миші Microsoft Office [Версія]** і виберіть команду **Змінити > відновлення з мережі**.

Якщо жоден із цих рішень не підійшов, докладніший список рішень можна знайти в статті служби підтримки, двічі клацнувши файл, [Office не](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)відкривається.
