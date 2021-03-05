---
title: Konfigurowanie usługi inicjowania obsługi administracyjnej
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482874"
---
# <a name="configuring-the-provision-service"></a>Konfigurowanie usługi inicjowania obsługi administracyjnej

Aby automatyczne inicjowanie obsługi użytkowników działało, usługa Azure AD wymaga prawidłowych poświadczeń, które umożliwiają jej połączenie się z interfejsem API usług sieci Web Workday. Ponadto przycisk Testuj połączenie w dniu roboczy z aplikacją inicjowania obsługi użytkowników usługi AD sprawdza również, czy może nawiązać połączenie z agentem inicjowania obsługi programu Azure AD Connect skojarzonym z domeną usługi AD.

Jeśli podczas zapisywania poświadczeń w portalu Azure Portal jest zwracany komunikat o błędzie, wykonaj poniższe zalecane czynności:

1. Upewnij się, że skonfigurowano konto użytkownika systemu integracji dni roboczych zgodnie z sekcją samouczka Konfigurowanie użytkownika systemu integracji [w programie Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Upewnij się, że usługa agenta inicjowania obsługi administracyjnej Azure AD Connect jest uruchomiona na lokalnym serwerze systemu Windows przy użyciu konsoli zarządzania usług. Możesz również sprawdzić stan agenta w portalu Azure Portal, klikając przycisk Wyświetl agentów lokalnych.
3. Upewnij się, że wartość pola "Nazwa użytkownika w dni robocze" jest wprowadzana w formacie username@workday-nazwa_dzierżawy. Jeśli brakuje nazwy dzierżawy w dni robocze, uwierzytelnianie w dni robocze kończy się niepowodzeniem.
4. Jeśli konfigurujesz integrację z dzierżawą implementacji Workday, zwróć uwagę na zaplanowane godziny przestojów dzierżawy w dni robocze. W dzień roboczy zaplanowano skrócenie czasu implementacji w weekendy (zwykle od piątku wieczór do soboty rano), a awarie łączności podczas tego okna przestojów są znanym problemem, który rozwiązuje automatycznie zaraz po powrocie dzierżawy implementacji do trybu online.
5. W rzadkich przypadkach ten błąd może być również wyświetlany, jeśli hasło użytkownika systemu integracji zostało zmienione ze względu na odświeżenie dzierżawy lub jeśli konto jest zablokowane lub wygasło. Sprawdź stan użytkownika systemu integracji z administratorem dni roboczych.

Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego [dla automatycznego inicjowania obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
