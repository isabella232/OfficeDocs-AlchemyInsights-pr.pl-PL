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
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330382"
---
# <a name="device-in-pending-state"></a>Urządzenie w stanie oczekiwania

**Wymagania wstępne:**

1. Jeśli używasz rejestracji urządzeń po raz pierwszy, sprawdź Wprowadzenie do zarządzania urządzeniami w usłudze [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) które pomoże Ci uzyskać informacje o tym, jak uzyskać urządzenia pod kontrolą usługi Azure AD.
2. Jeśli rejestrujesz urządzenia bezpośrednio w usłudze Azure AD i zapisujesz je w usłudze Intune, musisz najpierw upewnić się, że skonfigurowano usługę [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i że w pierwszej kolejności są [one](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) stosowane.
3. Upewnij się, że masz uprawnienia do wykonywania operacji w usłudze Azure AD i lokalnej usłudze AD. Tylko administrator globalny w usłudze Microsoft Azure Active Directory może zarządzać ustawieniami w przypadku rejestracji urządzeń. Jeśli dodatkowo konfigurujesz automatyczne rejestracje w lokalnej usłudze Active Directory, musisz być administratorem usługi Active Directory i usług federacyjnych Active Directory (o ile mają zastosowanie).

Proces rejestracji dołączania do hybrydowego programu Azure AD wymaga, aby urządzenia trafiły do sieci firmowej. Ta funkcja działa również przez sieć VPN, ale istnieje do tego kilka zastrzeżeniem. Słyszeliśmy, że w okolicznościach pracy zdalnej klienci potrzebują pomocy przy rozwiązywaniu problemów z hybrydowym procesem rejestracji dołączania do usługi Azure AD.

**Środowisko uwierzytelniania w chmurze (za pomocą synchronizacji skrótów haseł usługi Azure AD lub uwierzytelniania przekazać)**

Ten przepływ rejestracji jest również nazywany "sprzężeniami synchronizacji".

Oto zestawienie tego, co dzieje się podczas procesu rejestracji:

1. Windows 10 rekord punktu połączenia usługi (SCP), gdy użytkownik loguje się do urządzenia.

    1. Urządzenie najpierw próbuje pobrać informacje o dzierżawie z po stronie klienta SCP w rejestrze [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Aby uzyskać więcej informacji, zobacz [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. W przypadku niepowodzenia urządzenie komunikuje się z lokalną usługą Active Directory w celu uzyskania informacji o dzierżawie z ustawienia SCP. Aby zweryfikować SCP, zapoznaj się z tym [dokumentem.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Uwaga:** Zalecamy włączenie SCP w usłudze Active Directory i używanie tylko po stronie klienta na etapie weryfikacji wstępnej.

2. Windows 10 się z usługą Azure AD w kontekście systemowym w celu uwierzytelnienia się w usłudze Azure AD.

    Możesz sprawdzić, czy urządzenie może uzyskać dostęp do zasobów firmy Microsoft w ramach konta systemowego, używając skryptu Testuj łączność [z rejestracją urządzenia.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 wygeneruje certyfikat z podpisem własnym i przechowuje go pod obiektem komputera w lokalnej usłudze Active Directory. Wymaga to ujednania Kontroler domeny.

4. Obiekt urządzenia z certyfikatem jest synchronizowany z usługą Azure AD za pośrednictwem usługi Azure AD Połączenie. Domyślnie cykl synchronizacji trwa co 30 minut, ale to zależy od konfiguracji usługi Azure AD Połączenie. Aby uzyskać więcej informacji, zapoznaj się z tym [dokumentem.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Na tym etapie urządzenie z tematem powinno być w stanie **"** Oczekiwanie" w obszarze Urządzenie blade portalu Azure Portal.

6. Rejestracja zostanie zakończona przy następnym logowaniu Windows 10 użytkownika.

    **Uwaga:** Jeśli używasz sieci VPN, a logowanie/logowanie powoduje zakończenie łączności z domeną, możesz ręcznie wyzwolić rejestrację. W tym celu:
    
    Wydaj `dsregcmd /join` monit administratora lokalnego lub zdalnie za pośrednictwem programu PSExec na komputer.\
    Na przykład: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Aby uzyskać informacje o typowych Azure Active Directory rejestracji urządzeń, zobacz [Często zadawane pytania dotyczące urządzeń.](https://docs.microsoft.com/azure/active-directory/devices/faq)
