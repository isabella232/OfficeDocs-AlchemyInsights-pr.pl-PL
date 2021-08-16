---
title: Intune Exchange lokalnego łącznika
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
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013974"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokalnego łącznika

Aby uzyskać szczegółowe informacje dotyczące konfigurowania łącznika między usługą Intune a usługą Exchange, która jest hostowana lokalnie, zobacz następującą dokumentację:

[Konfigurowanie lokalnego łącznika usługi Intune Exchange w usłudze Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

P. Podczas próby skonfigurowania łącznika Exchange jest wyświetlany komunikat o błędzie, taki jak "Wersja dotykowa łącznika Exchange jest obsługiwana". Co może być przyczyną?

O. Konto, z których korzystasz, ma odpowiednią licencję — musi mieć aktywną licencję usługi Intune

P. Czy można mieć wiele łączników Exchange łączników?

O. Można skonfigurować tylko jeden łącznik usługi Exchange dla dzierżawy usługi Intune w Exchange organizacji. Łącznik można zainstalować tylko na jednym serwerze w organizacji wymiany wielu serwerów.

Nie można też skonfigurować łączników zarówno dla Exchange lokalnym, jak i dla Exchange Online w tej samej dzierżawie.

P. Czy łącznik może używać tablicy CAS jako połączenia z Exchange?

O. Określenie tablicy CAS nie jest obsługiwaną konfiguracją łącznika. W pliku konfiguracji łącznika, który można znaleźć w pliku konfiguracji łącznika, należy określić tylko jeden serwer i go

program data\microsoft\microsoft Intune on-premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Znajdź następujący wpis i ```<ExchangeWebServiceURL />``` zamień adres URL na serwer programu Exchange.

**Przykład:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Zapoznaj się z następującą dokumentacją, aby uzyskać dodatkowe rozwiązania problemów: Rozwiązywanie problemów z lokalnym łącznikiem sieci Exchange [Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Włączanie szczegółowego rejestrowania dla łącznika Exchange danych**

1. Otwórz plik Exchange konfiguracji śledzenia łącznika do edycji.  
Plik znajduje się w witrynie: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Przykład:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Znajdź element TraceSourceLine przy użyciu następującego klucza: OnPremisesExchangeConnectorService  
  
3. Zmienianie wartości węzła SourceLevel z Information ActivityTracing (wartość domyślna) na Verbose ActivityTracing  

**Przykład:**
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
4. Ponowne uruchamianie Microsoft Intune Exchange sieciowej  
5. Pełna synchronizacja w portalu Usługi Intune aż do jej zakończenia, a następnie ponowne zmienienie pliku XML na "Information ActivityTracing" i ponowne uruchomienie Microsoft Intune Exchange danych.  
6. Lokalizacja dzienników jest: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`