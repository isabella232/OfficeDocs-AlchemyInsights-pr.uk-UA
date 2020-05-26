---
title: 'AIP сканер: установка і конфігурація'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358570"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP сканер: установка і конфігурація

**Щоб встановити сканер AIP, дотримуйтеся рекомендованих рекомендацій**:

1. Якщо ви оновлюєте і не виконуєте чисту інсталяцію, переконайтеся, що ви виконали вказівки з [оновлення сканера захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) і для уніфікованого позначення клієнта, перегляньте [оновлення сканера захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Переконайтеся, що ви дотримуєтесь всіх [параметрів брандмауера та настройок мережної інфраструктури](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Переконайтеся, що для [політики встановлено](https://docs.microsoft.com/azure/information-protection/configure-policy) автоматичне маркування або підпис за промовчанням у політиці.
4. Переконайтеся, що відповідний тип файлу настроєно для міток/захисту, як описано в [типах файлів, які підтримуються клієнтом захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Крім того, якщо потрібно змінити поведінку за промовчанням, дотримуйтеся наведених нижче вказівок. [змінення рівня захисту файлів за промовчанням](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Переконайтеся, що обліковий запис користувача, настроєний для запуску служби сканера, має дозволи на доступ до всіх настроєних сховищ.
6. Якщо виникають проблеми, будь ласка, експортуйте журнали сканера та додайте їх до квитка підтримки.

**Експортування журналів сканера захисту інформації Azure**

1. Перейдіть до%Localappdate%\miceptemclinn, під контекстом користувача, який працює служба сканера.
2. ZIP весь вміст у папці MSIP.
3. Збережіть журнали на вибір місцеположення та Прикріпіть їх до вашого запиту на обслуговування.
4. Ви також можете використовувати [експорт-Aiplмоги-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**За додатковою інформацією див**.:
- [Розгортання в Azure захисту інформації сканер для автоматичної класифікації та захисту файлів](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Укажіть та використайте параметр маркерів для параметра Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Запуск циклу виявлення та перегляд звітів для сканера](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Огляд документації з захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Вимоги для захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Завантажити клієнт для захисту інформації Azure](https://www.microsoft.com/download/details.aspx?id=53018)
