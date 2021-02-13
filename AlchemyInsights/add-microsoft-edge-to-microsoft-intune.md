---
title: Додавання Microsoft EDGE до Microsoft InTune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194580"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a>Додавання Microsoft EDGE до Microsoft InTune

Щоб мати змогу розгортати, настроювати, відстежувати та захищати Microsoft EDGE для Windows 10, спочатку потрібно додати її до Microsoft InTune.

> [!IMPORTANT]
- Inune підтримує Microsoft EDGE 77 і новіші версії.
- Inune виявляє всі попередньо доступні інсталяції Microsoft EDGE.
- Якщо Microsoft EDGE інстальовано в контексті користувача, інсталяція системи призведе до перезаписування інсталяції в контексті користувача.
- Якщо Microsoft EDGE інстальовано в системному контексті, буде повідомлено про успішність інсталяції.
- Попередньо інстальовані Microsoft EDGE 77 і пізніші версії, для всіх каналів у контексті користувача буде замінено Microsoft EDGE, інстальованим в системному контексті.

**Передумовою**

Windows 10 версії 1709 або пізніші версії

**Кроки, щоб додати край до Inune**

1. [Настройте програму в програмі Inune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
2. [Настройте відомості про програму](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
3. [Настроювання параметрів програми](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
4. [Виберіть теги області (необов'язково)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
5. [Додайте програму](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).

Докладні відомості наведено в статті [Виправлення неполадок](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).




