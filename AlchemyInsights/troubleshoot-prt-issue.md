---
title: Rozwiązywanie problemu z PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573722"
---
# <a name="troubleshoot-prt-issue"></a>Rozwiązywanie problemu z PRT

W przypadku wszystkich urządzeń, które mogą dokończyć uwierzytelnianie, należy w pełni zarejestrować i w odpowiednim stanie i móc uzyskać podstawowy token odświeżania (PRT).

Proces rejestracji hybrydowej dołączania Azure AD wymaga, aby urządzenia były w sieci firmowej. Działa również w sieci VPN, ale istnieją pewne zastrzeżenia. Przesłuchamy klientów potrzebujących pomocy w rozwiązywaniu problemów dotyczących procesu rejestracji hybrydowych funkcji dołączania usługi Azure AD w ramach sytuacji zdalnej. Poniżej przedstawiono podział tego, co się dzieje w trakcie procesu rejestracji.

**Środowisko uwierzytelniania w chmurze (Korzystanie z synchronizacji skrótu hasła w usłudze Azure AD lub uwierzytelniania przekazujące)**

Ten przepływ rejestracji jest również nazywany "przyłączeniem do synchronizacji".

1. System Windows 10 odnajduje rekord punktu SCP po zalogowaniu się użytkownika do urządzenia.
    1. Urządzenie najpierw usiłuje pobrać informacje o dzierżawie ze strony klienta usługi SCP w rejestrze [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Aby uzyskać więcej informacji, zobacz ten [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Jeśli to nie uda, urządzenie komunikuje się z lokalną usługą Active Directory (AD), aby uzyskać informacje o dzierżawie od punktu połączenia usługi (SCP). Aby zweryfikować punkt SCP, zapoznaj się z tym [dokumentem](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Zalecamy włączenie punktu SCP w REKLAMie i korzystanie tylko z funkcji SCP po stronie klienta w celu wstępnego sprawdzania poprawności.

2. System Windows 10 próbuje komunikować się z usługą Azure AD w kontekście systemowym, aby uwierzytelnić się w usłudze Azure AD. Możesz sprawdzić, czy urządzenie może uzyskać dostęp do zasobów firmy Microsoft w ramach konta system przy użyciu skryptu łączności urządzenia testowego.

3. System Windows 10 wygeneruje certyfikat z podpisem własnym i zapisuje go pod obiektem komputera w usłudze AD — lokalnie. Wymaga to, aby kontroler domeny był oparty na linii.

4. Obiekt urządzenia z certyfikatem jest synchronizowany z usługą Azure AD za pośrednictwem usługi Azure AD Connect. Cykl synchronizacji jest domyślnie co 30 minut, ale zależy od konfiguracji usługi Azure AD Connect. Aby uzyskać więcej informacji, zapoznaj się z tym [dokumentem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Na tym etapie powinno być możliwe wyświetlenie urządzenia subject w stanie "oczekujące" w obszarze Kaseta urządzenia usługi Azure Portal.

6. Po następnym zalogowaniu się użytkownika do systemu Windows 10 rejestracja zostanie zakończona. 

> [!NOTE]
> Jeśli korzystasz z sieci VPN, a proces logowania wylogowania zakończy działanie połączenia z domeną, możesz wyzwolić rejestrację ręcznie:
 1. Wydaj dsregcmd/Join lokalnie na monit administratora lub zdalnie za pośrednictwem PSExec na Twój komputer. Na przykład PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Aby uzyskać więcej informacji o problemach z dołączaniem hybrydowym, zobacz [Rozwiązywanie problemów z urządzeniami](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
