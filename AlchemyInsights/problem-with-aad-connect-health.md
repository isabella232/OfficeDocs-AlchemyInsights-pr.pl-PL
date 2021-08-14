---
title: Problem z kondycją Połączenie AAD
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923762"
---
# <a name="problem-with-aad-connect-health"></a>Problem z kondycją Połączenie AAD

- Upewnij się, że masz upoważnienie do wykonania operacji. Administratorzy globalni mają domyślnie dostęp. Ponadto możesz użyć kontroli dostępu opartej na rolach, [aby](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegować uprawnienia rejestracji do współautora.
- Upewnij się, że wymagane punkty końcowe są włączone i nie są blokowane z powodu zapory. Aby uzyskać szczegółowe informacje, zobacz [wymagania.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Rejestracja może zakończyć się niepowodzeniem, ponieważ komunikacja wychodząca jest poddawana inspekcji SSL przez warstwę sieciową.
- Upewnij się, że zostały zweryfikowane ustawienia powiadomień dla usługi Azure AD Połączenie Health. Sprawdź swoje ustawienia. Ten [przewodnik](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pomoże Ci dowiedzieć się, jak skonfigurować ustawienia powiadomień dla usługi Azure AD Połączenie kondycji.
- Aby dowiedzieć się więcej o raporcie synchronizacji kondycji Połączenie AAD i sposobu jego pobierania, zobacz [Raport synchronizacji na poziomie obiektów.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Aby rozwiązać problemy z alertami kondycji usługi AAD Połączenie, postępuj zgodnie z instrukcje rozwiązywania problemów dotyczące alertów kondycji usługi [AAD Połączenie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Kondycja oraz w przypadku często zadawanego pytania, zobacz Typowe pytania dotyczące instalacji usługi [AAD Połączenie Kondycja.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
