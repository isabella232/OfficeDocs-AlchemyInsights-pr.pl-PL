---
title: Centrum administracyjne aplikacji Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354098"
---
# <a name="teams-admin-center"></a>Centrum administracyjne aplikacji Teams

Dowiedz się, jak zarządzać aplikacją Teams za pomocą [Centrum administracyjnego aplikacji Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jeśli nie możesz uzyskać dostępu do Centrum administracyjnego aplikacji Teams, sprawdź następujące elementy:

- Sprawdź, czy zezwolono na korzystanie z odpowiednich [adresów IP i URL usługi Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na dowolnych urządzeniach obwodowych (zaporze itp.) lub w zasadach zapory skonfigurowanych na maszynie lokalnej.
- Sprawdź, czy identyfikator logowania, z którego korzystasz, aby uzyskać dostęp do Portalu administracyjnego aplikacji Teams, odpowiada nazwie użytkownika wymienionej na liście w [portalu administracyjnym platformy Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Jeżeli w Centrum administracyjnym aplikacji Teams nie widać użytkowników, sprawdź następujące kwestie:

- Czy w ciągu ostatnich 24 godzin utworzono użytkowników lub przypisano licencje? Odczekaj co najmniej 24 godziny, zanim zgłosisz się do pomocy technicznej o wsparcie.
- Sprawdź, czy przypisano odpowiednie licencje.
- Jeśli masz lokalną usługę Active Directory, sprawdź, czy [wartość adresu msRTCSIP-PrimaryUserAddress lub adresu SIP w polu ProxyAddresses w lokalnej usłudze Active Directory jest unikatowa, a format pasuje](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) do sip: Nazwa**użytkownika** z [centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Jeśli zamierzasz zachować wdrożenie programu Skype dla firm Server i użytkownicy są lokalni i online: wykonaj **"Konfigurowanie hybrydowej z usługą Teams i Skype dla firm Online"** w Panelu sterowania serwera programu Skype dla firm i przenieś użytkowników w trybie online.
