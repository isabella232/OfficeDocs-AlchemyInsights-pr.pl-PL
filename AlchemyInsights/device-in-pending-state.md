---
title: Urządzenie w stanie oczekiwania
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679987"
---
# <a name="device-in-pending-state"></a>Urządzenie w stanie oczekiwania

**Dotyczących**

1. Jeśli konfigurujesz rejestracje urządzeń po raz pierwszy, upewnij się, że zostały przejrzane [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , które pomogą Ci w tym, jak uzyskać urządzenia objęte kontrolą usługi Azure AD.
2. Jeśli rejestrujesz urządzenia w usłudze Azure AD bezpośrednio i rejestrujesz je w usłudze Intune, musisz upewnić się, że [skonfigurowano usługę Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) , a w pierwszej kolejności należy wprowadzić [licencję](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Upewnij się, że masz autoryzację do wykonywania operacji w usłudze Azure AD i w lokalnej usłudze AD. Tylko administrator globalny w usłudze Azure AD może zarządzać ustawieniami rejestracji urządzeń. Ponadto w przypadku konfigurowania rejestracji automatycznej w lokalnej usłudze Active Directory musisz być administratorem usługi Active Directory i usługami AD FS (jeśli jest dostępna).

Proces rejestracji hybrydowej dołączania Azure AD wymaga, aby urządzenia były w sieci firmowej. Działa również w sieci VPN, ale istnieją pewne zastrzeżenia. Mamy do tego, aby klienci musieli uzyskać pomoc w rozwiązywaniu problemów dotyczących procesu rejestracji hybrydowej funkcji dołączania usługi Azure AD w ramach zdalnego środowiska roboczego.

**Środowisko uwierzytelniania w chmurze (Korzystanie z synchronizacji skrótu hasła w usłudze Azure AD lub uwierzytelniania przekazujące)**

Ten przepływ rejestracji jest również nazywany "przyłączeniem do synchronizacji".

Poniżej przedstawiono podział na to, co się dzieje w trakcie procesu rejestracji:

1. System Windows 10 odnajduje rekord punktu połączenia usługi (SCP), gdy użytkownik loguje się do urządzenia.

    1. Urządzenie najpierw usiłuje pobrać informacje o dzierżawie ze strony klienta usługi SCP w rejestrze [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Aby uzyskać więcej informacji, zobacz [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Jeśli to nie uda, urządzenie komunikuje się z lokalną usługą Active Directory, aby uzyskać informacje o dzierżawie z punktu połączenia usługi. Aby zweryfikować punkt SCP, należy odwołać się do tego [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Zalecamy włączenie punktu połączenia usługi w usłudze Active Directory i korzystanie tylko z usługi SCP po stronie klienta w celu wstępnego sprawdzania poprawności.

2. System Windows 10 próbuje komunikować się z usługą Azure AD w kontekście systemowym, aby uwierzytelnić się w usłudze Azure AD.

    Możesz sprawdzić, czy urządzenie może uzyskać dostęp do zasobów firmy Microsoft w ramach konta system przy użyciu [skryptu łączności urządzenia testowego](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. System Windows 10 generuje certyfikat z podpisem własnym i przechowuje go w obszarze obiektu komputer w usłudze Active Directory lokalnego. Wymaga to, aby kontroler domeny był oparty na linii.

4. Obiekt urządzenia z certyfikatem zostanie zsynchronizowany z usługą Azure AD za pośrednictwem usługi Azure AD Connect. Cykl synchronizacji jest domyślnie co 30 minut, ale zależy od konfiguracji usługi Azure AD Connect. Aby uzyskać więcej informacji, zapoznaj się z tym [dokumentem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Na tym etapie powinno być możliwe wyświetlenie urządzenia subject w stanie "**oczekujące**" w obszarze Kaseta urządzenia usługi Azure Portal.

6. Po następnym zalogowaniu się użytkownika do systemu Windows 10 rejestracja zostanie zakończona.

    > [!NOTE]
    > Jeśli korzystasz z sieci VPN, a wylogowanie/logowanie zakończy łączność z domeną, możesz wyzwolić rejestrację ręcznie. W tym celu:
    >
    > Wygeneruj `dsregcmd /join` lokalnie monit administratora lub zdalnie, korzystając z PSExec na komputerze.
    >
    > Na przykład: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Aby poznać typowe problemy dotyczące rejestracji urządzeń usługi Azure Active Directory, zobacz [często zadawane pytania dotyczące urządzeń](https://docs.microsoft.com/azure/active-directory/devices/faq).
