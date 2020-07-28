---
title: Змінення каналів оновлення для програм Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440025"
---
# <a name="change-update-channels-for-office-apps"></a>Змінення каналів оновлення для програм Office

Для нових офісних установок використовуйте настройки завантаження програмного забезпечення Office, щоб вибрати потрібний канал оновлення, а потім інсталювати (або повторно інсталювати) програми Office. Додаткові відомості наведено в розділі [керування налаштуваннями завантаження програмного забезпечення в Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Зверніть увагу** Канал оновлення, вибраний за допомогою настройок завантаження програмного забезпечення Office, застосовується до всіх користувачів, які виконують нові інсталяції за допомогою порталу O365. Для отримання додаткових відомостей див. [завантаження та інсталяція або повторна інсталяція Microsoft 365 або Office 2019 на ПК або Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Для існуючих офісних установок використовуйте засіб розгортання Office (ODT), щоб перейти до іншого каналу оновлення:  

1. Завантажити останню версію засобу розгортання Office (setup.exe) з [центру завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Визначте назву каналу, до якого потрібно перейти. Для отримання додаткових відомостей див. [Параметри настроювання засобу розгортання Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Створення XML-файлу конфігурації з указанням відповідного імені каналу, наприклад update.xml.  
    є. <Configuration>  
    B. <оновлення **каналу = "щомісяця"** />  
    C. </Configuration>
4. У командному рядку в режимі адміністратора перейдіть до розташування папки, де setup.exe проживає та виконайте таку команду:  
    є. setup.exe/настроювання update.xml
5. Запустіть застосунок Office (наприклад, Excel) **і виберіть**  >  **обліковий запис**. У розділі відомості про продукт виберіть оновити **Параметри**  >  **Update Now**.

Щоб отримати додаткові відомості, Дізнайтеся, [як змінити канали оновлення для наявних програм Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Для перемикання оновлень каналів для вибраної групи користувачів або за допомогою диспетчера конфігурацій (SCCM), настройте параметри каналу оновлення за допомогою GPO. Щоб отримати додаткові відомості див. [Огляд каналів оновлення для Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Докладніше про [керування каналами Office 365 ProPlus для фахівців з інформаційних технологій](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) і [керування оновленнями для Microsoft 365 Apps за допомогою диспетчера конфігурацій Microsoft endPoint](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).