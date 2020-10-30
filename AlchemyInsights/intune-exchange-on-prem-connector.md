---
title: Inune Exchange для локальної сполучної лінії
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808137"
---
# <a name="intune-exchange-on-premise-connector"></a>Inune Exchange для локальної сполучної лінії

Щоб отримати докладні відомості про настроювання сполучної лінії між Inune та Exchange, які розміщуються локально, ознайомтеся з такими документами:

[Настроювання з'єднувача локального сервера Exchange у Microsoft Inune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**ЗАПИТАННЯ Й відповіді**

П: під час спроби настроювання сполучної лінії Exchange з'являється повідомлення про помилку, наприклад "версія з'єднувача Exchange не підтримується". Що може бути причиною?

В: обліковий запис, який ви використовуєте, ліцензовано належним чином – вона має бути активною ліцензією Inune

Запитання: чи можна мати кілька сполучних ліній Exchange?

В: можна настроїти лише один з'єднувач Exchange для клієнта Inune за організацію Exchange. З'єднувач можна інсталювати лише на одному сервері в організації з кількома серверами Exchange Server.

Крім того, ви не можете налаштувати сполучні лінії для Exchange для локального та Exchange Online, настроєного в одному клієнті.

З: чи може сполучна лінія використовувати масив CAS як підключення до Exchange?

В: зазначення масиву CAS не підтримується в настройках з'єднувача. Потрібно вказати лише один сервер і має бути жорстко вказано в файлі конфігурації з'єднувача, який можна знайти в

Програма data\microsoft\microsoft InTune для локального з'єднувача Exchange \OnpremiseExchangeConnectorServiceConfiguration.xml

Знайдіть наведений нижче запис ```<ExchangeWebServiceURL />``` і замініть URL-адресу на сервері Exchange.

**Наприклад**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Щоб отримати додаткові виправлення неполадок, ознайомтеся з наведена нижче документацією: [Виправлення неполадок локальної сполучної лінії Exchange](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Увімкнення детального журналювання для з'єднувача Exchange**

1. Відкрийте файл конфігурації трасування з'єднувача Exchange для редагування.  
Файл розташовано за адресою:%Programdata%\microsoft\ Windows Inune Exchange Connector\TracingConfiguration.xml  

**Наприклад**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Знайдіть TraceSourceLine з таким ключем: OnPremisesExchangeConnectorService  
  
3. Змінення значення вузла SourceLevel з інформаційних ActivityTracing (за замовчуванням) для докладного ActivityTracing  

**Наприклад**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Перезапуск служби Exchange для Microsoft Inune  
5. Повна синхронізація на порталі Inune, доки не завершиться, а потім знову змініть його на "відомості ActivityTracing", а потім перезапустіть службу Microsoft Inune Exchange.  
6. Розташування журналів: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`