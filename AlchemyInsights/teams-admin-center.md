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
# <a name="teams-admin-center"></a><span data-ttu-id="a4e8b-102">Centrum administracyjne aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="a4e8b-102">Teams Admin Center</span></span>

<span data-ttu-id="a4e8b-103">Dowiedz się, jak zarządzać aplikacją Teams za pomocą [Centrum administracyjnego aplikacji Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a4e8b-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="a4e8b-104">Jeśli nie możesz uzyskać dostępu do Centrum administracyjnego aplikacji Teams, sprawdź następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="a4e8b-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="a4e8b-105">Sprawdź, czy zezwolono na korzystanie z odpowiednich [adresów IP i URL usługi Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na dowolnych urządzeniach obwodowych (zaporze itp.) lub w zasadach zapory skonfigurowanych na maszynie lokalnej.</span><span class="sxs-lookup"><span data-stu-id="a4e8b-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="a4e8b-106">Sprawdź, czy identyfikator logowania, z którego korzystasz, aby uzyskać dostęp do Portalu administracyjnego aplikacji Teams, odpowiada nazwie użytkownika wymienionej na liście w [portalu administracyjnym platformy Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a4e8b-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="a4e8b-107">Jeżeli w Centrum administracyjnym aplikacji Teams nie widać użytkowników, sprawdź następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="a4e8b-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="a4e8b-108">Czy w ciągu ostatnich 24 godzin utworzono użytkowników lub przypisano licencje?</span><span class="sxs-lookup"><span data-stu-id="a4e8b-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="a4e8b-109">Odczekaj co najmniej 24 godziny, zanim zgłosisz się do pomocy technicznej o wsparcie.</span><span class="sxs-lookup"><span data-stu-id="a4e8b-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="a4e8b-110">Sprawdź, czy przypisano odpowiednie licencje.</span><span class="sxs-lookup"><span data-stu-id="a4e8b-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="a4e8b-111">Jeśli korzystasz z lokalnej usługi Active Directory, upewnij się, że [wartość msRTCSIP-PrimaryUserAddress lub adres SIP w polu proxyAddresses w lokalnej usłudze Active Directory jest unikatowy, a format pasuje](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) do SIP:**username** użytkownika w [centrum administracyjnym Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a4e8b-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="a4e8b-112">Jeśli zamierzasz zachować wdrożenie programu Skype dla firm i korzystać z nich lokalnie i w trybie online, postępuj zgodnie z instrukcjami **"Konfigurowanie hybrydowe za pomocą zespołów i usługi Skype dla firm Online"** w panelu sterowania programu Skype dla firm i przenoszenie użytkowników w trybie online.</span><span class="sxs-lookup"><span data-stu-id="a4e8b-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
