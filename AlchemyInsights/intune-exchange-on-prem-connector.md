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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="05857-102">Inune Exchange для локальної сполучної лінії</span><span class="sxs-lookup"><span data-stu-id="05857-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="05857-103">Щоб отримати докладні відомості про настроювання сполучної лінії між Inune та Exchange, які розміщуються локально, ознайомтеся з такими документами:</span><span class="sxs-lookup"><span data-stu-id="05857-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="05857-104">Настроювання з'єднувача локального сервера Exchange у Microsoft Inune Azure</span><span class="sxs-lookup"><span data-stu-id="05857-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="05857-105">**ЗАПИТАННЯ Й відповіді**</span><span class="sxs-lookup"><span data-stu-id="05857-105">**FAQ:**</span></span>

<span data-ttu-id="05857-106">П: під час спроби настроювання сполучної лінії Exchange з'являється повідомлення про помилку, наприклад "версія з'єднувача Exchange не підтримується".</span><span class="sxs-lookup"><span data-stu-id="05857-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="05857-107">Що може бути причиною?</span><span class="sxs-lookup"><span data-stu-id="05857-107">What could be the cause?</span></span>

<span data-ttu-id="05857-108">В: обліковий запис, який ви використовуєте, ліцензовано належним чином – вона має бути активною ліцензією Inune</span><span class="sxs-lookup"><span data-stu-id="05857-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="05857-109">Запитання: чи можна мати кілька сполучних ліній Exchange?</span><span class="sxs-lookup"><span data-stu-id="05857-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="05857-110">В: можна настроїти лише один з'єднувач Exchange для клієнта Inune за організацію Exchange.</span><span class="sxs-lookup"><span data-stu-id="05857-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="05857-111">З'єднувач можна інсталювати лише на одному сервері в організації з кількома серверами Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="05857-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="05857-112">Крім того, ви не можете налаштувати сполучні лінії для Exchange для локального та Exchange Online, настроєного в одному клієнті.</span><span class="sxs-lookup"><span data-stu-id="05857-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="05857-113">З: чи може сполучна лінія використовувати масив CAS як підключення до Exchange?</span><span class="sxs-lookup"><span data-stu-id="05857-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="05857-114">В: зазначення масиву CAS не підтримується в настройках з'єднувача.</span><span class="sxs-lookup"><span data-stu-id="05857-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="05857-115">Потрібно вказати лише один сервер і має бути жорстко вказано в файлі конфігурації з'єднувача, який можна знайти в</span><span class="sxs-lookup"><span data-stu-id="05857-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="05857-116">Програма data\microsoft\microsoft InTune для локального з'єднувача Exchange \OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="05857-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="05857-117">Знайдіть наведений нижче запис ```<ExchangeWebServiceURL />``` і замініть URL-адресу на сервері Exchange.</span><span class="sxs-lookup"><span data-stu-id="05857-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="05857-118">**Наприклад**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="05857-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="05857-119">Щоб отримати додаткові виправлення неполадок, ознайомтеся з наведена нижче документацією: [Виправлення неполадок локальної сполучної лінії Exchange](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="05857-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="05857-120">**Увімкнення детального журналювання для з'єднувача Exchange**</span><span class="sxs-lookup"><span data-stu-id="05857-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="05857-121">Відкрийте файл конфігурації трасування з'єднувача Exchange для редагування.</span><span class="sxs-lookup"><span data-stu-id="05857-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="05857-122">Файл розташовано за адресою:%Programdata%\microsoft\ Windows Inune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="05857-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="05857-123">**Наприклад**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="05857-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="05857-124">Знайдіть TraceSourceLine з таким ключем: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="05857-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="05857-125">Змінення значення вузла SourceLevel з інформаційних ActivityTracing (за замовчуванням) для докладного ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="05857-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="05857-126">**Наприклад**</span><span class="sxs-lookup"><span data-stu-id="05857-126">**Example:**</span></span>
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
4. <span data-ttu-id="05857-127">Перезапуск служби Exchange для Microsoft Inune</span><span class="sxs-lookup"><span data-stu-id="05857-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="05857-128">Повна синхронізація на порталі Inune, доки не завершиться, а потім знову змініть його на "відомості ActivityTracing", а потім перезапустіть службу Microsoft Inune Exchange.</span><span class="sxs-lookup"><span data-stu-id="05857-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="05857-129">Розташування журналів: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="05857-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>