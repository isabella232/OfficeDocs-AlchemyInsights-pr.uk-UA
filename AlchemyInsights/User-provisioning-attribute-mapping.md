---
title: Зіставлення атрибутів користувача
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949900"
---
# <a name="user-provisioning-attribute-mapping"></a>Зіставлення атрибутів користувача

1. Щоб виправити помилки, які мають відомі проблеми з відображенням атрибутів, ознайомтеся з [зіставленнями атрибутів](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Служба Microsoft Azure Active Directory (AD) надає підтримку для підготовки користувачів стороннім програмам SaaS, як-от "Salesforce", "G Suite" тощо. Якщо ви активувати підготовку користувача для програми SaaS для третьої сторони, на порталі Azure можна керувати значеннями атрибутів за допомогою зіставлень атрибутів. Щоб дізнатися, як настроїти зіставлення атрибутів за замовчуванням, перегляньте статтю [Настроювання атрибута підготовки користувачів – зіставлення для програм SaaS у службі Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Докладні відомості про підготовку користувачів за програмою SaaS можна дізнатися про [те, що таке автоматизована програма підготовки користувачів SaaS в Лазурне AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Під час настроювання зіставлення атрибутів для підготовки користувача може виявитися, що атрибут, який потрібно зіставити, не відображається у списку вихідних атрибутів. [Атрибут Sync від локального служби Active Directory до Azure AD для підготовки до програми у](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) статті показано, як додати відсутній атрибут, синхронізуючи її з локального рекламного повідомлення в Azure AD.
