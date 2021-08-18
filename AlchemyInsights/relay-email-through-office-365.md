---
title: Przekazywanie wiadomości e-mail przez platformę Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898558"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Konfiguracja urządzenia wielofunkcyjnego lub aplikacji do wysyłania wiadomości e-mail

Aby poznać dostępne opcje i instrukcje, zobacz [Jak skonfigurować urządzenie wielofunkcyjne lub aplikację do wysyłania wiadomości e-mail przy użyciu platformy Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Jeśli masz urządzenie lub aplikację, która ostatnio przestała działać, najczęstszymi problemami są:

- **Błędy związane z uwierzytelnianiem podczas korzystania z przesyłania klienta uwierzytelniania SMTP** Ostatnio wpisano pewne zmiany dotyczące działania uwierzytelniania SMTP. Aby uzyskać więcej informacji na temat rozwiązywania problemów, zobacz sekcję rozwiązywanie problemów z uwierzytelnianiem za pomocą [drukarki, skanerów](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)i aplikacji biznesowych, które wysyłają wiadomości e-mail za pomocą usługi Microsoft 365 lub Office 365.
- Podczas bezpiecznego połączenia z usługą ILS akceptujemy tylko wersję **TLS 1.2 Office 365** Jeśli korzystasz z bezpiecznego połączenia (TLS), upewnij się, że urządzenie aplikacji obsługuje TLS 1.2. Aby uzyskać więcej informacji, zobacz Przygotowywanie się do [1.2 TLS](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)w programie Office 365 i Office 365 GCC.
 
Aby uzyskać informacje na temat innych problemów i ich rozwiązań, zobacz Rozwiązywanie problemów z drukarkami, skanerami i aplikacjami LOB, które wysyłają wiadomości [e-mail](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)przy użyciu Microsoft 365 lub Office 365.

Aby wyświetlić urządzenia, na których występuje problem, przejdź do [raportu Klienci uwierzytelniania SMTP](https://protection.office.com/mailflow/dashboard).

**Uwaga:** Exchange Online scenariuszy z wysyłką zbiorczą. Aby wysyłać masową komercyjną pocztę e-mail (na przykład biuletyny klientów), należy korzystać z usług innych dostawców.
