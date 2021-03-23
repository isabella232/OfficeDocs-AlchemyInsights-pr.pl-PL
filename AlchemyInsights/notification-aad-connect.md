---
title: Notification AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037230"
---
# <a name="notification-aad-connect"></a>Notification AAD Connect

- Upewnij się, że masz upoważnienie do wykonania operacji. Administratorzy globalni mają domyślnie dostęp. Ponadto możesz użyć kontroli dostępu opartej na rolach, [aby](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegować uprawnienia rejestracji do współautora.
- Upewnij się, że wymagane punkty końcowe są włączone i nie są blokowane z powodu zapory. Aby uzyskać szczegółowe informacje, zobacz [wymagania.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Rejestracja może zakończyć się niepowodzeniem, ponieważ komunikacja wychodząca jest poddawana inspekcji SSL przez warstwę sieciową.
- Upewnij się, że zostały zweryfikowane ustawienia powiadomień dotyczące usługi Azure AD Connect Health, i sprawdź ustawienia. Aby dowiedzieć się, jak skonfigurować ustawienia powiadomień dla powiadomień usługi Azure AD Connect Health, zobacz ten [przewodnik.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Aby dowiedzieć się więcej na temat raportu synchronizacji usługi AAD Connect Health i sposobu jego pobierania, zobacz Raport [synchronizacji na poziomie obiektów.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Aby rozwiązać problemy z alertami kondycji usługi AAD Connect, postępuj zgodnie z instrukcje rozwiązywania problemów dotyczące alertów o odświeżeń danych [aAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) oraz w przypadku często zadawanego pytania, zobacz Typowe pytania dotyczące instalacji usługi [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
