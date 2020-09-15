---
title: Служба Active Directory не синхронізується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697650"
---
# <a name="active-directory-not-syncing"></a>Служба Active Directory не синхронізується

Якщо ви отримуєте помилки синхронізації, наприклад "без нещодавньої синхронізації", або зверніть увагу на стан синхронізації служби каталогів на порталі адміністрування Office, говориться: "Востаннє синхронізовано більше 3 днів тому", можливо, це означає, що AADConnect має неправильні настройки або недостатні дозволи для виконання синхронізації.  

Повторна інсталяція AADConnect за допомогою функції Експрес-параметрів може швидко вирішити проблему:

1. [Завантажте найновішу версію AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Виконайте вказівки з інсталяції Експрес](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)-програми.

Щоб отримати докладніші відомості про облікові записи служби AADConnect, перегляньте статтю [Azure AD Connect: облікові записи та дозволи](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
