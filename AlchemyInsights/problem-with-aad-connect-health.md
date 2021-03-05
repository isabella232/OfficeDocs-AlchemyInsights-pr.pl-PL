---
title: Problem z kondycją połączenia AAD
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482073"
---
# <a name="problem-with-aad-connect-health"></a>Problem z kondycją połączenia AAD

- Upewnij się, że masz upoważnienie do wykonywania operacji. Administratorzy globalni mają domyślnie dostęp. Ponadto możesz użyć kontroli dostępu opartej na rolach, [aby](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegować uprawnienia rejestracji do współautora.
- Upewnij się, że wymagane punkty końcowe są włączone i nie są blokowane z powodu zapory. Aby uzyskać szczegółowe informacje, zobacz [wymagania.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Rejestracja może zakończyć się niepowodzeniem ze względu na to, że komunikacja wychodząca podlega inspekcji SSL przez warstwę sieciową.
- Upewnij się, że ustawienia powiadomień dotyczące usługi Azure AD Connect Health zostały zweryfikowane. Sprawdź swoje ustawienia. Ten [przewodnik](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) może ułatwić ci skonfigurowanie ustawień powiadomień dotyczących powiadomień dotyczących kondycji usługi Azure AD Connect.
- Aby dowiedzieć się więcej na temat raportu synchronizacji usługi AAD Connect Health i sposobu jego pobierania, zobacz raport synchronizacji [na poziomie obiektu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Aby rozwiązać problemy z alertami kondycji usługi AAD Connect, skorzystaj z przewodnika po rozwiązywaniu problemów dla alertów o odświeżaniu danych [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) oraz w przypadku często zadawanego pytania, zobacz typowe pytania dotyczące instalacji [usługi AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
