---
title: Konfigurowanie usługi synchronizacji mim
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481868"
---
# <a name="configure-mim-sync-service"></a>Konfigurowanie usługi synchronizacji mim

Usługa synchronizacji programu Microsoft Identity Manager (MIM) jest składnikiem funkcji MIM. Jest to scentralizowana usługa lokalna, która przechowuje i integruje informacje dla organizacji, które mają wiele lokalnych katalogów i baz danych. Być może uda się rozwiązać problem z synchronizacją MIM, jeśli ten problem został rozwiązany w ostatniej aktualizacji mim lub jest jednym z pozostałych problemów wymienionych w poniższej sekcji.

**Zalecane czynności**

1. Upewnij się, że korzystasz z ostatniej aktualizacji synchronizacji MIM, i sprawdź informacje o wersji synchronizacji [MIM,](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) aby ustalić, czy problem został rozwiązany w aktualizacji.
2. Jeśli problem dotyczy łącznika generic LDAP, Generic SQL, Lotus Domino lub Web Services, upewnij się, że używasz najnowszej aktualizacji łączników [ogólnych.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Jeśli synchronizacja miM zostanie zatrzymana z błędem, zapoznaj się z tabelą kodów błędów uruchamiania, aby ustalić potencjalne przyczyny. [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)
4. Jeśli po zatrzymaniu uruchamiania z wyjątkiem **biblioteki dll rozszerzenia,** kliknij te wyrazy, aby otworzyć okno właściwości obiektu spacji łącznika, a następnie kliknij pozycję Śledzenie **stosu...** aby wyświetlić więcej informacji na temat przyczyny, zgodnie z opisem w bibliotece [DLL-Rozszerzenia,](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)wyjątek. 
5. Jeśli składnik usługi powiadomień o zmianie hasła (PCNS, Password Change Notification Service) zgłasza błąd **6025** w dzienniku zdarzeń podczas synchronizacji haseł, zapoznaj się z podręcznikiem, aby uzyskać informacje na temat rozwiązywania problemów z błędem raportowania [PCNS 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Jeśli pełna synchronizacja z agentem zarządzania usługami FIM jest wolna, sprawdź ustawienie automatycznego powiększania dla pliku TempDB zgodnie z opisem w rozwiązywaniu problemów z wolno lub wysunięciem [pełnej synchronizacji.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) 
7. Jeśli wystąpi błąd zatrzymano-serwer z usługami sieci Web, których tworzenie zakończyło się niepowodzeniem przy użyciu agenta zarządzania usługami FIM, zobacz informacje o pomocy [technicznej: failed-creation-via-web-services,](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) aby uzyskać omówienie przyczyn.

