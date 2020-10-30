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
# <a name="intune-exchange-on-premise-connector"></a>Łącznik lokalny w usłudze Intune Exchange

Aby uzyskać szczegółowe informacje dotyczące konfigurowania łącznika między usługami Intune i Exchange, które są hostowane lokalnie, zapoznaj się z poniższą dokumentacją:

[Konfigurowanie lokalnego łącznika programu Exchange w usłudze Intune na platformie Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

P: podczas próby skonfigurowania programu Exchange Connector jest wyświetlany komunikat o błędzie, na przykład "wersja łącznika programu Exchange Connector jest nieobsługiwana". Co może być przyczyną?

A: konto, którego używasz, jest licencjonowane, musi mieć aktywną licencję usługi Intune.

P: Czy można korzystać z wielu łączników programu Exchange?

O: możesz skonfigurować jeden łącznik programu Exchange dla każdego dzierżawy usługi Intune dla każdej organizacji programu Exchange. Łącznik można zainstalować tylko na jednym serwerze w organizacji programu Exchange Server.

Ponadto nie można korzystać z łączników skonfigurowanych zarówno w programie Exchange lokalny, jak i w usłudze Exchange Online skonfigurowanej w tej samej dzierżawie.

P: czy łącznik ma używać tablicy CAS jako połączenia z programem Exchange?

A: określenie tablicy CAS nie jest obsługiwaną konfiguracją w konfiguracji łącznika. Należy określić tylko jeden serwer i należy go Anglojęzyczna w pliku konfiguracji łącznika, który można znaleźć w

Program Data\Microsoft\Microsoft Intune na lokalnym łączniku programu Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Zlokalizuj Poniższy wpis ```<ExchangeWebServiceURL />``` i Zastąp adres URL serwerem Exchange.

**Przykłady**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Aby uzyskać dodatkowe informacje dotyczące rozwiązywania problemów, zapoznaj się z następującą dokumentacją: [Rozwiązywanie problemów z lokalnym łącznikiem Exchange w usłudze Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Włączanie pełnego rejestrowania w programie Exchange Connector**

1. Otwórz plik konfiguracji śledzenia łącznika programu Exchange do edycji.  
Lokalizacja pliku:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Przykłady**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Znajdź TraceSourceLine z następującym kluczem: OnPremisesExchangeConnectorService  
  
3. Zmień wartość SourceLevel Node z ActivityTracing informacji (ustawienie domyślne) na verbose ActivityTracing  

**Przykłady**
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
4. Ponowne uruchamianie usługi programu Microsoft Intune Exchange  
5. Pełna synchronizacja w portalu Intune do momentu jego zakończenia, a następnie zmienienie kodu XML z powrotem na "Information ActivityTracing" i ponowne uruchomienie usługi Exchange w usłudze Microsoft Intune.  
6. Lokalizacja dzienników to: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`