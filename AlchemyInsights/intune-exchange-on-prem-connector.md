---
title: Intune Exchange on-premise Connector
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013985"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange on-premise Connector

Докладні відомості про налаштування з'єднатора між Intune Exchange розміщеною локально, див. в цій документації:

[Налаштування локального з'єднатора Exchange Intune в Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Запитання й відповіді:**

П. Під час спроби налаштувати з'єдн Exchange язковий з'єднач відображається повідомлення про помилку Exchange версія з'єднатора. У чому могла бути причина?

В. Обліковий запис, який ви використовуєте, ліцензовано відповідним чином – він має активну ліцензію Intune

Запитання. Чи можна мати кілька сполучних Exchange з'єдначів?

В. Для кожного клієнта Intune можна налаштувати Exchange лише один з'єдн Exchange організації. З'єднник можна інсталювати лише на одному сервері в організації обміну кількома серверами.

Крім того, в одному й тому самому Exchange не можна налаштувати з'єдн Exchange Online в одному й тому самому клієнта.

Запитання. Чи може з'єднувати сполучна Exchange за допомогою масиву CAS?

В. Вибір масиву CAS не підтримується в налаштуванні з'єднатора. Потрібно вказати лише один сервер, і його потрібно вказати у файлі конфігурації з'єднатора, який можна знайти в

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Знайдіть наведений нижче ```<ExchangeWebServiceURL />``` запис і замініть URL-адресу сервером Exchange.

**Приклад:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Додаткові способи виправлення неполадок див. в наведеній нижче документації. Виправлення неполадок із локальним з'єднатором [Intune Exchange'](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Увімкнення журналювання в усьому Exchange з'єднувача**

1. Відкрийте файл конфігурації Exchange З'єднатора для редагування.  
Файл розташовано за такою: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Приклад:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Знайдіть програму TraceSourceLine за допомогою такого розділу: OnPremisesExchangeConnectorService.  
  
3. Змініть значення вузла SourceLevel з Information ActivityTracing (за замовчуванням) на Verbose ActivityTracing  

**Приклад.**
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
4. Перезапустіть Microsoft Intune Exchange служби  
5. Повна синхронізація на порталі Intune до завершення, а потім знову змініть XML на "Information ActivityTracing" (Трасування даних) і перезапустіть Microsoft Intune Exchange Service.  
6. Розташування журналів: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`