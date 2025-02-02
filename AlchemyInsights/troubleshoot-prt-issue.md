---
title: Rozwiązywanie problemów z PRT
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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330969"
---
# <a name="troubleshoot-prt-issue"></a>Rozwiązywanie problemów z PRT

Aby każde urządzenie ukończyć uwierzytelnienie, musi ono być w pełni zarejestrowane i w dobrym stanie oraz mieć możliwość uzyskania podstawowego tokenu odświeżania (PRT).

Hybrydowy proces rejestracji dołączania do usługi Azure AD wymaga, aby urządzenia trafiły do sieci firmowej. Ta funkcja działa również przez sieć VPN, ale istnieje do tego kilka zastrzeżeniem. W warunkach pracy zdalnej słyszeliśmy, że klienci potrzebują pomocy przy rozwiązywaniu problemów z hybrydowym procesem rejestracji dołączania do usługi Azure AD. Oto zestawienie tego, co dzieje się "w sobie" podczas procesu rejestracji.

**Środowisko uwierzytelniania w chmurze (za pomocą synchronizacji skrótów haseł usługi Azure AD lub uwierzytelniania przekazać)**

Ten przepływ rejestracji jest również nazywany "sprzężeniami synchronizacji".

1. Windows 10 rekord SCP po zalogowaniu się użytkownika na urządzeniu.
    1. Urządzenie najpierw próbuje pobrać informacje o dzierżawie z po stronie klienta SCP w rejestrze [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. W przypadku awarii urządzenie komunikuje się z lokalną usługą Active Directory (AD), aby uzyskać informacje o dzierżawie z punktu połączenia usługi (SCP). Aby zweryfikować SCP, zapoznaj się z tym [dokumentem.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Uwaga:** Zalecamy włączenie SCP w uceniu AD i używanie tylko po stronie klienta SCP w celu wstępnej weryfikacji.

2. Windows 10 się z usługą Azure AD w kontekście systemowym w celu uwierzytelnienia się w usłudze Azure AD. Możesz sprawdzić, czy urządzenie może uzyskać dostęp do zasobów firmy Microsoft w ramach konta systemowego, używając skryptu Testuj łączność z rejestracją urządzenia.

3. Windows 10 wygeneruje certyfikat z podpisem własnym i przechowuje go pod obiektem komputera w lokalnej u usługi AD. Wymaga to ujednania Kontroler domeny.

4. Obiekt urządzenia z certyfikatem jest synchronizowany z usługą Azure AD za pośrednictwem usługi Azure AD Połączenie. Domyślnie cykl synchronizacji jest co 30 minut, ale zależy to od konfiguracji usługi Azure AD Połączenie. Aby uzyskać więcej informacji, zapoznaj się z tym [dokumentem.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Na tym etapie urządzenie tematu powinno być widzieć w stanie "Oczekiwanie" w obszarze Urządzenie blade portalu Azure Portal.

6. Podczas następnego logowania użytkownika Windows 10 rejestracja zostanie zakończona. 

**Uwaga:** Jeśli używasz sieci VPN i proces logowania przez logowanie kończy łączność z domeną, możesz ręcznie wyzwolić rejestrację:
 1. Wydaj monit dsregcmd /join lokalnie w administracyjnym lub zdalnie za pośrednictwem programu PSExec na komputer. Na przykład PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Aby uzyskać więcej szczegółowych informacji o problemach dotyczących dołączania hybrydowego, zobacz [Rozwiązywanie problemów z urządzeniami.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
