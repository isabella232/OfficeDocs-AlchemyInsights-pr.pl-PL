---
title: Centrum administracyjne aplikacji Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670374"
---
# <a name="teams-admin-center"></a>Centrum administracyjne aplikacji Teams

Dowiedz się, jak zarządzać aplikacją Teams za pomocą [Centrum administracyjnego aplikacji Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jeśli nie możesz uzyskać dostępu do Centrum administracyjnego aplikacji Teams, sprawdź następujące elementy:

- Sprawdź, czy zezwolono na korzystanie z odpowiednich [adresów IP i URL usługi Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na dowolnych urządzeniach obwodowych (zaporze itp.) lub w zasadach zapory skonfigurowanych na maszynie lokalnej.
- Sprawdź, czy identyfikator logowania, z którego korzystasz, aby uzyskać dostęp do Portalu administracyjnego aplikacji Teams, odpowiada nazwie użytkownika wymienionej na liście w [portalu administracyjnym platformy Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Jeżeli w Centrum administracyjnym aplikacji Teams nie widać użytkowników, sprawdź następujące kwestie:

- Czy w ciągu ostatnich 24 godzin utworzono użytkowników lub przypisano licencje? Odczekaj co najmniej 24 godziny, zanim zgłosisz się do pomocy technicznej o wsparcie.
- Sprawdź, czy przypisano odpowiednie licencje.
- Jeśli korzystasz z lokalnej usługi Active Directory, upewnij się, że [wartość msRTCSIP-PrimaryUserAddress lub adres SIP w polu proxyAddresses w lokalnej usłudze Active Directory jest unikatowy, a format pasuje](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) do SIP:**username** użytkownika w [centrum administracyjnym Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Jeśli zamierzasz zachować wdrożenie programu Skype dla firm i korzystać z nich lokalnie i w trybie online, postępuj zgodnie z instrukcjami **"Konfigurowanie hybrydowe za pomocą zespołów i usługi Skype dla firm Online"** w panelu sterowania programu Skype dla firm i przenoszenie użytkowników w trybie online.
