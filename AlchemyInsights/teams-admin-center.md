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
# <a name="teams-admin-center"></a><span data-ttu-id="383b9-102">Centrum administracyjne aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="383b9-102">Teams Admin Center</span></span>

<span data-ttu-id="383b9-103">Dowiedz się, jak zarządzać aplikacją Teams za pomocą [Centrum administracyjnego aplikacji Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="383b9-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="383b9-104">Jeśli nie możesz uzyskać dostępu do Centrum administracyjnego aplikacji Teams, sprawdź następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="383b9-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="383b9-105">Sprawdź, czy zezwolono na korzystanie z odpowiednich [adresów IP i URL usługi Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na dowolnych urządzeniach obwodowych (zaporze itp.) lub w zasadach zapory skonfigurowanych na maszynie lokalnej.</span><span class="sxs-lookup"><span data-stu-id="383b9-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="383b9-106">Sprawdź, czy identyfikator logowania, z którego korzystasz, aby uzyskać dostęp do Portalu administracyjnego aplikacji Teams, odpowiada nazwie użytkownika wymienionej na liście w [portalu administracyjnym platformy Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="383b9-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="383b9-107">Jeżeli w Centrum administracyjnym aplikacji Teams nie widać użytkowników, sprawdź następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="383b9-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="383b9-108">Czy w ciągu ostatnich 24 godzin utworzono użytkowników lub przypisano licencje?</span><span class="sxs-lookup"><span data-stu-id="383b9-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="383b9-109">Odczekaj co najmniej 24 godziny, zanim zgłosisz się do pomocy technicznej o wsparcie.</span><span class="sxs-lookup"><span data-stu-id="383b9-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="383b9-110">Sprawdź, czy przypisano odpowiednie licencje.</span><span class="sxs-lookup"><span data-stu-id="383b9-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="383b9-111">Jeśli masz lokalną usługę Active Directory, sprawdź, czy [wartość adresu msRTCSIP-PrimaryUserAddress lub adresu SIP w polu ProxyAddresses w lokalnej usłudze Active Directory jest unikatowa, a format pasuje](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) do sip: Nazwa**użytkownika** z [centrum administracyjnego usługi Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="383b9-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="383b9-112">Jeśli zamierzasz zachować wdrożenie programu Skype dla firm Server i użytkownicy są lokalni i online: wykonaj **"Konfigurowanie hybrydowej z usługą Teams i Skype dla firm Online"** w Panelu sterowania serwera programu Skype dla firm i przenieś użytkowników w trybie online.</span><span class="sxs-lookup"><span data-stu-id="383b9-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
