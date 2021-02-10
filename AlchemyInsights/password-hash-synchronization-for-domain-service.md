---
title: Синхронізація хеш-пароля для служби domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177617"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Синхронізація хеш-пароля для служби domain

**Якщо у вашому екземплярі Azure AD DS з'являється запит на ввімкнення функції гешування паролів**

Ви зіткнулися з сценарієм, у якому ви працюєте з гібридним середовищем, щоб користувачі могли синхронізувати їх із локального середовища служб домену Azure Active Directory (AD DS). Цей сценарій трапляється, незважаючи на те, що під час синхронізації пароля в локальній службі AD DS для свого клієнта Azure відображається синхронізація паролів.

**Спричиняють**

Ця дія відбувається через те, що за замовчуванням для Azure AD Connect не синхронізуватиметься новий Диспетчер технологій LAN Manager (NTLM) і пароль протоколу Kerberos, необхідні для Azure AD DS.

**Спосіб вирішення** 

Щоб синхронізувати ці хеш-суми, необхідні для автентифікації NTLM та Kerberos, потрібно настроїти підключення Azure AD.

Після настроювання служби Azure AD Connect, створення локального облікового запису або подія змінення пароля також синхронізує дані про застарілі паролі в лазуркому ОГОЛОШЕННІ. Щоб отримати докладніші відомості про це та вказівки про те, як увімкнути синхронізацію паролів у гібридному середовищі Azure AD DS, ознайомтеся з наведеними [нижче](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) відомостями.