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
# <a name="configuring-the-provision-service"></a><span data-ttu-id="e27ad-102">Konfigurowanie usługi inicjowania obsługi administracyjnej</span><span class="sxs-lookup"><span data-stu-id="e27ad-102">Configuring the Provision service</span></span>

<span data-ttu-id="e27ad-103">Aby automatyczne inicjowanie obsługi użytkowników działało, usługa Azure AD wymaga prawidłowych poświadczeń, które umożliwiają jej połączenie się z interfejsem API usług sieci Web Workday.</span><span class="sxs-lookup"><span data-stu-id="e27ad-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="e27ad-104">Ponadto przycisk Testuj połączenie w dniu roboczy z aplikacją inicjowania obsługi użytkowników usługi AD sprawdza również, czy może nawiązać połączenie z agentem inicjowania obsługi programu Azure AD Connect skojarzonym z domeną usługi AD.</span><span class="sxs-lookup"><span data-stu-id="e27ad-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="e27ad-105">Jeśli podczas zapisywania poświadczeń w portalu Azure Portal jest zwracany komunikat o błędzie, wykonaj poniższe zalecane czynności:</span><span class="sxs-lookup"><span data-stu-id="e27ad-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="e27ad-106">Upewnij się, że skonfigurowano konto użytkownika systemu integracji dni roboczych zgodnie z sekcją samouczka Konfigurowanie użytkownika systemu integracji [w programie Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="e27ad-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="e27ad-107">Upewnij się, że usługa agenta inicjowania obsługi administracyjnej Azure AD Connect jest uruchomiona na lokalnym serwerze systemu Windows przy użyciu konsoli zarządzania usług.</span><span class="sxs-lookup"><span data-stu-id="e27ad-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="e27ad-108">Możesz również sprawdzić stan agenta w portalu Azure Portal, klikając przycisk Wyświetl agentów lokalnych.</span><span class="sxs-lookup"><span data-stu-id="e27ad-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="e27ad-109">Upewnij się, że wartość pola "Nazwa użytkownika w dni robocze" jest wprowadzana w formacie username@workday-nazwa_dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="e27ad-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="e27ad-110">Jeśli brakuje nazwy dzierżawy w dni robocze, uwierzytelnianie w dni robocze kończy się niepowodzeniem.</span><span class="sxs-lookup"><span data-stu-id="e27ad-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="e27ad-111">Jeśli konfigurujesz integrację z dzierżawą implementacji Workday, zwróć uwagę na zaplanowane godziny przestojów dzierżawy w dni robocze.</span><span class="sxs-lookup"><span data-stu-id="e27ad-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="e27ad-112">W dzień roboczy zaplanowano skrócenie czasu implementacji w weekendy (zwykle od piątku wieczór do soboty rano), a awarie łączności podczas tego okna przestojów są znanym problemem, który rozwiązuje automatycznie zaraz po powrocie dzierżawy implementacji do trybu online.</span><span class="sxs-lookup"><span data-stu-id="e27ad-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="e27ad-113">W rzadkich przypadkach ten błąd może być również wyświetlany, jeśli hasło użytkownika systemu integracji zostało zmienione ze względu na odświeżenie dzierżawy lub jeśli konto jest zablokowane lub wygasło.</span><span class="sxs-lookup"><span data-stu-id="e27ad-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="e27ad-114">Sprawdź stan użytkownika systemu integracji z administratorem dni roboczych.</span><span class="sxs-lookup"><span data-stu-id="e27ad-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="e27ad-115">Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego [dla automatycznego inicjowania obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="e27ad-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
