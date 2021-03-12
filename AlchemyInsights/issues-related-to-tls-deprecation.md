---
title: Nie można wysyłać/odbierać wiadomości e-mail do/z usługi Office 365 z powodu wyłączenia TLS 1.0 i TLS 1.1
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747121"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="16a44-102">Nie można wysyłać/odbierać wiadomości e-mail do/z usługi Office 365 z powodu wyłączenia TLS 1.0 i TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="16a44-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="16a44-103">Jak potwierdzi to wpis w centrum wiadomości MC229914, ALS 1.0 i TLS 1.1, rozpoczął wymuszanie punktów końcowych przepływu poczty usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="16a44-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="16a44-104">Wkrótce usługa Office 365 nie będzie już akceptować połączeń poczty e-mail TLS 1.0 i TLS 1.1 ze źródeł zewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="16a44-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="16a44-105">Ponadto usługi Exchange Online nigdy nie będą używać TLS 1.0 lub 1.1 do wysyłania wychodzących wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="16a44-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="16a44-106">Jeśli występują problemy z powodu wyłączenia usługi TLS 1.0 lub 1.1, może wystąpić jeden z następujących błędów:</span><span class="sxs-lookup"><span data-stu-id="16a44-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="16a44-107">Nadawca wraca do wiadomości o niedostarczeniu — '421 4.4.2 Połączenie zostało przerwane z powodu socketError'</span><span class="sxs-lookup"><span data-stu-id="16a44-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="16a44-108">Błąd w podglądzie kolejki serwera lokalnego, który wysyła wiadomość e-mail do specjalisty 365— '421 4.4.2 Połączenie zostało przerwane z powodu błędu SocketError'</span><span class="sxs-lookup"><span data-stu-id="16a44-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="16a44-109">Błąd w dzienniku Send connector [Protocol (Wyślij](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) protokół łącznika) na serwerze wysyłającym wiadomość e-mail do usługi Office 365 — niepowodzenie negocjacji protokołu TLS z błędem SocketError</span><span class="sxs-lookup"><span data-stu-id="16a44-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="16a44-110">Błąd w dzienniku wysyłania lub odbierania protokołu łącznika — '451 5.7.3 Należy najpierw uruchomić polecenie STARTTLS.</span><span class="sxs-lookup"><span data-stu-id="16a44-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="16a44-111">Jeśli występują jakiekolwiek z powyższych błędów, upewnij się, że serwer, który wysyła lub odbiera pocztę e-mail, ma włączoną obsługę TLS 1.2, sprawdzając następujące klucze rejestru.</span><span class="sxs-lookup"><span data-stu-id="16a44-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="16a44-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Klient] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="16a44-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="16a44-113">Jeśli w powyższych kluczach rejestru zostaną wprowadzone jakiekolwiek zmiany w celu włączenia usługi TLS 1.2, uruchom ponownie serwer, aby zmiany zaczęły obowiązywać.</span><span class="sxs-lookup"><span data-stu-id="16a44-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="16a44-114">Upewnij się też, że masz zainstalowane najnowsze aktualizacje systemu Windows i programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="16a44-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="16a44-115">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="16a44-115">For more information, see:</span></span>

- [<span data-ttu-id="16a44-116">Exchange Server TLS, część 1: Przygotowanie się na TLS 1.2 — społeczność techniczna firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="16a44-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="16a44-117">Exchange Server wskazówek dotyczących usługi TLS Część 2: Włączanie usługi TLS 1.2 i identyfikowania klientów, którzy jej nie używa, — społeczność techniczna firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="16a44-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="16a44-118">Opis scenariuszy obsługi poczty e-mail, jeśli nie można ustalić wersji TLS z usługą Exchange Online — społeczność techniczna firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="16a44-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
