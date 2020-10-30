---
title: Łącznik lokalny w usłudze Intune Exchange
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
ms.contentlocale: pl-PL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808146"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="7a196-102">Łącznik lokalny w usłudze Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="7a196-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="7a196-103">Aby uzyskać szczegółowe informacje dotyczące konfigurowania łącznika między usługami Intune i Exchange, które są hostowane lokalnie, zapoznaj się z poniższą dokumentacją:</span><span class="sxs-lookup"><span data-stu-id="7a196-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="7a196-104">Konfigurowanie lokalnego łącznika programu Exchange w usłudze Intune na platformie Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="7a196-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="7a196-105">**FAQ:**</span><span class="sxs-lookup"><span data-stu-id="7a196-105">**FAQ:**</span></span>

<span data-ttu-id="7a196-106">P: podczas próby skonfigurowania programu Exchange Connector jest wyświetlany komunikat o błędzie, na przykład "wersja łącznika programu Exchange Connector jest nieobsługiwana".</span><span class="sxs-lookup"><span data-stu-id="7a196-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="7a196-107">Co może być przyczyną?</span><span class="sxs-lookup"><span data-stu-id="7a196-107">What could be the cause?</span></span>

<span data-ttu-id="7a196-108">A: konto, którego używasz, jest licencjonowane, musi mieć aktywną licencję usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="7a196-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="7a196-109">P: Czy można korzystać z wielu łączników programu Exchange?</span><span class="sxs-lookup"><span data-stu-id="7a196-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="7a196-110">O: możesz skonfigurować jeden łącznik programu Exchange dla każdego dzierżawy usługi Intune dla każdej organizacji programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a196-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="7a196-111">Łącznik można zainstalować tylko na jednym serwerze w organizacji programu Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="7a196-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="7a196-112">Ponadto nie można korzystać z łączników skonfigurowanych zarówno w programie Exchange lokalny, jak i w usłudze Exchange Online skonfigurowanej w tej samej dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="7a196-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="7a196-113">P: czy łącznik ma używać tablicy CAS jako połączenia z programem Exchange?</span><span class="sxs-lookup"><span data-stu-id="7a196-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="7a196-114">A: określenie tablicy CAS nie jest obsługiwaną konfiguracją w konfiguracji łącznika.</span><span class="sxs-lookup"><span data-stu-id="7a196-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="7a196-115">Należy określić tylko jeden serwer i należy go Anglojęzyczna w pliku konfiguracji łącznika, który można znaleźć w</span><span class="sxs-lookup"><span data-stu-id="7a196-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="7a196-116">Program Data\Microsoft\Microsoft Intune na lokalnym łączniku programu Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="7a196-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="7a196-117">Zlokalizuj Poniższy wpis ```<ExchangeWebServiceURL />``` i Zastąp adres URL serwerem Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a196-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="7a196-118">**Przykłady**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="7a196-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="7a196-119">Aby uzyskać dodatkowe informacje dotyczące rozwiązywania problemów, zapoznaj się z następującą dokumentacją: [Rozwiązywanie problemów z lokalnym łącznikiem Exchange w usłudze Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="7a196-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="7a196-120">**Włączanie pełnego rejestrowania w programie Exchange Connector**</span><span class="sxs-lookup"><span data-stu-id="7a196-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="7a196-121">Otwórz plik konfiguracji śledzenia łącznika programu Exchange do edycji.</span><span class="sxs-lookup"><span data-stu-id="7a196-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="7a196-122">Lokalizacja pliku:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="7a196-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="7a196-123">**Przykłady**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="7a196-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="7a196-124">Znajdź TraceSourceLine z następującym kluczem: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="7a196-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="7a196-125">Zmień wartość SourceLevel Node z ActivityTracing informacji (ustawienie domyślne) na verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="7a196-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="7a196-126">**Przykłady**</span><span class="sxs-lookup"><span data-stu-id="7a196-126">**Example:**</span></span>
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
4. <span data-ttu-id="7a196-127">Ponowne uruchamianie usługi programu Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="7a196-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="7a196-128">Pełna synchronizacja w portalu Intune do momentu jego zakończenia, a następnie zmienienie kodu XML z powrotem na "Information ActivityTracing" i ponowne uruchomienie usługi Exchange w usłudze Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7a196-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="7a196-129">Lokalizacja dzienników to: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="7a196-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>