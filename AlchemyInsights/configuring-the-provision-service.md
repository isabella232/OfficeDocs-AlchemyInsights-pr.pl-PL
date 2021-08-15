---
title: Konfigurowanie usługi inicjowania obsługi
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033288"
---
# <a name="configuring-the-provision-service"></a>Konfigurowanie usługi inicjowania obsługi

Aby automatyczne inicjowanie obsługi administracyjnej użytkowników działało, usługa Azure AD wymaga prawidłowych poświadczeń, które umożliwiają jej połączenie z interfejsem API usług sieci Web Workday. Ponadto przycisk Testuj połączenie w dniu roboczy do aplikacji inicjowania obsługi użytkowników usługi AD sprawdza również, czy można połączyć się z agentem inicjowania obsługi administracyjnej usługi Azure AD Połączenie skojarzonym z domeną usługi AD.

Jeśli portal Azure Portal zwraca błąd po zapisaniu poświadczeń, wykonaj poniższe zalecane czynności:

1. Upewnij się, że skonfigurowano konto użytkownika systemu integracji dni roboczych zgodnie z sekcją samouczka Konfigurowanie użytkownika systemu integracji [w dni robocze.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Upewnij się, że usługa Azure AD Połączenie agenta inicjowania obsługi administracyjnej jest uruchomiona na lokalnym Windows przy użyciu konsoli zarządzania usługami. Możesz również sprawdzić stan agenta w portalu Azure Portal, klikając przycisk Wyświetl agentów lokalnych.
3. Upewnij się, że wartość pola "Workday Username" jest wprowadzana w username@workday nazwa_dzierżawy. Jeśli brakuje nazwy dzierżawy w dni robocze, uwierzytelnianie w dni robocze kończy się niepowodzeniem.
4. Jeśli konfigurujesz integrację z dzierżawą implementacji dni roboczych, zwróć uwagę na zaplanowane godziny przestojów dzierżawy w dni robocze. W ciągu weekendów (zwykle od piątku wieczór do soboty rano) czas implementacji dzierżawcy został zaplanowany na ułamek w dół, a awarie łączności podczas tego okna przestojów to znany problem, który automatycznie rozwiązuje się zaraz po powrocie dzierżawy implementacji do trybu online.
5. W rzadkich przypadkach ten błąd może być również wyświetlany, jeśli hasło użytkownika systemu integracji zostało zmienione w wyniku odświeżenia dzierżawy lub gdy konto jest zablokowane lub wygasło. Sprawdź stan użytkownika systemu Integration System wraz z administratorem dni roboczych.

Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego dla [automatycznego inicjowania obsługi użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
