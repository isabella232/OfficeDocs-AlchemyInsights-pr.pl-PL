---
title: Nie można wysyłać/odbierać wiadomości e-mail do/z Office 365 z powodu wyłączenia TLS 1.0 i TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054916"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nie można wysyłać/odbierać wiadomości e-mail do/z Office 365 z powodu wyłączenia TLS 1.0 i TLS 1.1

Jak potwierdzono w centrum wiadomości po wyczycie mc229914, kodów TLS 1.0 i TLS 1.1, rozpoczęto wymuszanie dla punktów końcowych przepływu Exchange Online poczty e-mail. Wkrótce Office 365 nie będzie już akceptować połączeń poczty e-mail TLS 1.0 i TLS 1.1 ze źródeł zewnętrznych. Ponadto Exchange Online poczty wychodzącej nie będzie używać adresów TLS 1.0 ani 1.1. Jeśli występują problemy z powodu wyłączenia usługi TLS 1.0 lub 1.1, może wystąpić jeden z następujących błędów:

- Nadawca wraca do wiadomości o niedostarczeniu — '421 4.4.2 Połączenie zostało przerwane z powodu socketError'
- Błąd w podglądzie kolejki serwera lokalnego, który wysyła wiadomość e-mail do specjalisty 365— '421 4.4.2 Połączenie zostało przerwane z powodu błędu SocketError'
- Błąd dziennika Send connector [Protocol (Wyślij](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) protokół łącznika) na serwerze wysyłającym wiadomość e-mail do Office 365 — nieudane negocjacje dotyczące protokołu TLS z błędem SocketError
- Błąd w dzienniku wysyłania lub odbierania protokołu łącznika — '451 5.7.3 Należy najpierw uruchomić polecenie STARTTLS.

Jeśli występują jakiekolwiek z powyższych błędów, upewnij się, że serwer, który wysyła lub odbiera pocztę e-mail, ma włączoną obsługę TLS 1.2, sprawdzając następujące klucze rejestru.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Klient] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Jeśli w powyższych kluczach rejestru zostaną wprowadzone jakiekolwiek zmiany w celu włączenia usługi TLS 1.2, uruchom ponownie serwer, aby zmiany zaczęły obowiązywać. Upewnij się też, że masz zainstalowane najnowsze Windows i Exchange aktualizacje.

Więcej informacji można znaleźć w następujących artykułach:

- [Exchange Server Wskazówki dotyczące usługi TLS, część 1. Przygotowanie się do 1.2 TLS — witryna techniczna firmy Microsoft Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Wskazówki dotyczące usługi TLS Część 2: Włączanie usługi TLS 1.2 i identyfikowania klientów, którzy jej nie używania — wskazówki techniczne firmy Microsoft Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Opis scenariuszy obsługi poczty e-mail, jeśli nie można ustalić wersji TLS za pośrednictwem Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
