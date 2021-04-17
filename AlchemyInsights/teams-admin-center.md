---
title: Centrum administracyjne aplikacji Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826389"
---
# <a name="teams-admin-center"></a>Centrum administracyjne aplikacji Teams

Dowiedz się, jak zarządzać aplikacją Teams za pomocą [Centrum administracyjnego aplikacji Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jeśli nie możesz uzyskać dostępu do Centrum administracyjnego aplikacji Teams, sprawdź następujące elementy:

- Sprawdź, czy zezwolono na korzystanie z odpowiednich [adresów IP i URL usługi Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na dowolnych urządzeniach obwodowych (zaporze itp.) lub w zasadach zapory skonfigurowanych na maszynie lokalnej.
- Sprawdź, czy identyfikator logowania, z którego korzystasz, aby uzyskać dostęp do Portalu administracyjnego aplikacji Teams, odpowiada nazwie użytkownika wymienionej na liście w [portalu administracyjnym platformy Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Jeżeli w Centrum administracyjnym aplikacji Teams nie widać użytkowników, sprawdź następujące kwestie:

- Czy w ciągu ostatnich 24 godzin utworzono użytkowników lub przypisano licencje? Odczekaj co najmniej 24 godziny, zanim zgłosisz się do pomocy technicznej o wsparcie.
- Sprawdź, czy przypisano odpowiednie licencje.
- Jeśli masz lokalną usługę Active Directory, sprawdź, czy wartość [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) lub adresu SIP w polu ProxyAddresses w lokalnej usłudze Active Directory jest unikatowa, a format jest taki jak **sip:** Nazwa użytkownika użytkownika z centrum administracyjnego platformy [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Jeśli zamierzasz zachować wdrożenie programu Skype dla firm Server i mieć użytkowników w domu oraz w trybie online: wykonaj czynności "Konfigurowanie wdrożenia hybrydowego z usługami Teams i Skype dla firm **Online"** w Panelu sterowania programu Skype dla firm Server i przenieś użytkowników do trybu online.
