---
title: Konfigurowanie dlp punktu końcowego
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555553"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="8fc0f-102">Konfigurowanie dlp punktu końcowego</span><span class="sxs-lookup"><span data-stu-id="8fc0f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="8fc0f-103">Program Microsoft Endpoint DLP umożliwia rozszerzenie funkcji ochrony i monitorowania DLP na poufne informacje na urządzeniach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="8fc0f-104">Po urządzenia są wbudowane w zarządzanie urządzeniami, można utworzyć zasady DLP, aby wymusić akcje ochronne na elementach.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="8fc0f-105">Eksplorator działań może służyć do monitorowania aktywności dla poufnych elementów.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="8fc0f-106">Aby uzyskać więcej informacji, zobacz [Włączanie urządzeń do zarządzania urządzeniami](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="8fc0f-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="8fc0f-107">Aby rozpocząć pracę z programem DLP punktu końcowego:</span><span class="sxs-lookup"><span data-stu-id="8fc0f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="8fc0f-108">Upewnij się, że masz odpowiednie licencje SKU/subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="8fc0f-109">Aby uzyskać więcej informacji, zobacz [Licencjonowanie jednostek SKU/subskrypcji](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="8fc0f-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="8fc0f-110">Sprawdź uprawnienia wymagane do umożliwienia zarządzania urządzeniami, dostępu do strony dołączania lub włączenia/wyłączenia monitorowania urządzenia.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="8fc0f-111">Aby uzyskać więcej informacji, zobacz [Uprawnienia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="8fc0f-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="8fc0f-112">Urządzenia wbudowane do zarządzania urządzeniami, wykonując procedurę dołączania urządzeń.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="8fc0f-113">Jeśli brakuje opcji Dołączanie do urządzenia (wersja zapoznawcza) w **obszarze Ustawienia**zgodności M365, upewnij się, że masz odpowiednią licencję i uprawnienia, o których mowa powyżej.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="8fc0f-114">Aby uzyskać więcej informacji, zobacz [Urządzenia dołączające](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="8fc0f-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="8fc0f-115">Tworzenie zasad DLP w celu ochrony poufnych elementów.</span><span class="sxs-lookup"><span data-stu-id="8fc0f-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="8fc0f-116">Aby uzyskać więcej informacji, zobacz [Scenariusze zasad DLP punktu końcowego](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="8fc0f-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="8fc0f-117">Aby uzyskać więcej informacji na temat dlp punktu końcowego firmy Microsoft, zobacz [Dowiedz się więcej o zapobieganiu utracie danych punktu końcowego systemu Microsoft 365 (wersja zapoznawcza).](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="8fc0f-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>