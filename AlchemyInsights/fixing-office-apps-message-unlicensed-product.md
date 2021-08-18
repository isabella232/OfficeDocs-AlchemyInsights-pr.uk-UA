---
title: Не вдається активувати Office
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
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327867"
---
# <a name="unable-to-activate-office"></a>Не вдається активувати Office

**Примітка.** Якщо використовується попередня версія Windows (наприклад, Windows 7), переконайтеся, що протокол TLS 1.2 ввімкнуто за замовчуванням. Докладні відомості див. в статтях Оновлення для ввімкнення [протоколів TLS 1.1 і TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)як безпечних протоколів за замовчуванням у WindowsHTTP у Windows.

- Перевірте, чи не минув термін дії передплати.
- Переконайтеся, що у вас є передплата, яка підтримує клієнтські ліцензії, як-от Office 365 Business або Office 365 Business преміум, і що [користувачу призначено ліцензію](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Переконайтеся, що користувач входить в Office за допомогою облікового запису, якому призначено ліцензію.
- Перегляньте [сторінку справності служб Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health), щоб перевірити наявність відомих проблем зі службою.
- Перевірте брандмауер, антивірусну програму та параметри проксі-сервера, щоб переконатися, що вони не блокують доступ програм Microsoft 365 до Інтернету. Див. статтю [Діапазони URL- і IP-адрес Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Діапазони URL- і IP-адрес Office 365").

**Порада.** На комп’ютерах із Windows ми можемо діагностувати та автоматично усунути кілька поширених проблем із входом у систему Office. Завантажте та запустіть  **[Помічник із підтримки й відновлення від Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**, щоб скористатися нашим автоматизованим інструментом.

Виконайте наступні дії з виправлення неполадок:

- Відкрийте програму Office і [вийдіть](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) з будь-якого наявного облікового запису користувача. [Видаліть](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) та [повторно призначте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ліцензію Office, а потім [увійдіть в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9), використовуючи обліковий запис користувача.
- Запустіть [Засіб вирішення проблем активації](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Скиньте стан активації Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Скидання стану активації Office")
- [Виконайте відновлення з мережі для пакета Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Додаткові способи виправлення неполадок див. в статтях:  

- [Помилки про "неліцензований продукт" і помилки активації в Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Помилка "На жаль, не вдалося підключитися до облікового запису. Спробуйте ще раз пізніше" під час активації Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)