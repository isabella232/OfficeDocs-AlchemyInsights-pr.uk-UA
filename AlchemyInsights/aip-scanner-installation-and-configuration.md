---
title: 'AIP scanner: installation and configuration'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821684"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP scanner: installation and configuration

**Щоб інсталювати сканер AIP, дотримуйтеся рекомендованих рекомендацій:**

1. Якщо ви виконуєте чисту інсталяцію, але не виконуєте чисту інсталяцію, переконайтеся, що ви дотримувалися рекомендацій з оновлення сканера [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) і клієнта уніфікованого підписування, див. номери оновлення засобу перевірки захисту даних [Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Переконайтеся, що ви відповідаєте всім вимогам до [брандмауерів і інфраструктури мережі.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Переконайтеся, [що політики настроєно на](https://docs.microsoft.com/azure/information-protection/configure-policy) автоматичне підписування, або призначте політикі стандартну мітку.
4. Переконайтеся, що для відповідного типу файлу настроєно етикетку або захист, як описано в розділі Типи файлів, які підтримує клієнт [Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Крім того, якщо потрібно змінити стандартну поведінку, дотримуйтеся наведених нижче порад: Змінення рівня захисту файлів [за замовчуванням.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Переконайтеся, що обліковий запис користувача, настроєний для запуску служби сканера, має дозволи на доступ до всіх налаштованих сховищ.
6. Якщо проблеми не зникнуть, експортуйте журнали сканера та додайте їх до запиту на підтримку.

**Експорт журналів засобу перевірки даних Azure**

1. Перейдіть до %localappdata%\Microsoft\MSIP у контексті користувача, який виконує службу сканера.
2. Запакувати весь вміст папки MSIP.
3. Збережіть журнали у вибраному розташуванні та вкладіть їх у свій запит на обслуговування.
4. Ви також можете використовувати [Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Докладні відомості див. в такому:**
- [Розгортання сканера Azure Information Protection для автоматичного класифікації та захисту файлів](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Визначення та використання параметра Token для Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Запуск циклу виявлення та перегляд звітів для сканера](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Перегляд документації для захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Вимоги до захисту даних в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Завантаження клієнта Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
