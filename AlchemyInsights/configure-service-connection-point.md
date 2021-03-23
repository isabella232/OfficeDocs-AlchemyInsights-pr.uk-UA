---
title: Настроювання точки з'єднання служби (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037293"
---
# <a name="configure-service-connection-point-scp"></a>Настроювання точки з'єднання служби (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c 001d/-2145648611)**

- **Причина**: не вдається прочитати об'єкт scp і отримати відомості про клієнта AZURE AD
- **Роздільна здатність**: посилання на розділ [Настроювання точки з'єднання служби](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**План дій**

- Перевірте, чи отримали пристрій GPO для контрольованого перевірки.
- Переконайтеся, що об'єкт групової політики створив розділи реєстру.
- Переконайтеся, що у вас є 2 клавіші, створені за допомогою ІДЕНТИФІКАТОРА каталогів і домену onmicrosoft.

**Настроювання клієнтського реєстру для SCP**

Використовуйте наведений нижче приклад, щоб створити об'єкт групової політики (GPO), щоб розгорнути параметр реєстру, який настроює запис SCP в реєстрі пристроїв.

1. Відкрийте консоль керування груповою політикою та створіть новий об'єкт групової політики в домені.
     - Надання новоствореного імені групової політики (наприклад, ClientSideSCP)

2. Відредагуйте об'єкт групової політики та знайдіть такий шлях: налаштування **конфігурації комп'ютера > > настройки Windows > реєстрі**.

3. Клацніть правою кнопкою миші **реєстр** та виберіть **елемент новий > реєстру**.

4. На вкладці **загальні** настройте наведені нижче дії.
  
- **Дія**: оновлення
    
- **Вулик**: HKEY_LOCAL_MACHINE
    
- **Шлях до ключа**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Ім'я значення**: tenantid
    
- **Тип значення**: REG_SZ
    
- **Значення даних**: GUID або ідентифікатор каталогу в екземплярі AZURE AD (це значення можна знайти на **порталі azure Portal > azure Active directory > властивості > ідентифікатор каталогу**)
 
- Натисніть кнопку **OK**.
 
5. Клацніть правою кнопкою миші **реєстр** та виберіть **елемент новий > реєстру**.

6. На вкладці **загальні** настройте наведені нижче дії.
  
- **Дія**: оновлення
    
- **Вулик**: HKEY_LOCAL_MACHINE
    
- **Шлях до ключа**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Ім'я _ значення**: ім'я для tenantname
    
- **Тип значення**: REG_SZ
    
- **Значення даних**: перевірену назву домену, якщо використовується інтегроване середовище, наприклад AD FS. Перевірену назву домену або ім'я домену onmicrosoft.com (наприклад, contoso. onmicrosoft). com, якщо використовується кероване середовище

- Натисніть кнопку **OK**.

7. Закрийте редактор для щойно створеного об'єкта групової політики.

8. Зв'яжіть щойно створений об'єкт групової політики, у якому містяться підключені до домену комп'ютери, які належать до списку контрольованих свиті.

Докладні відомості наведено в статті [контрольована перевірка гібридного AD JOIN-Azure Документи Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) і  [Виправлення неполадок із гібридним Лазурний Active Directory | Документи Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









