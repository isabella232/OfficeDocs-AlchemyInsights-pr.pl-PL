---
title: Problemy związane z siecią VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555231"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="c6a5a-102">Problemy związane z siecią VPN</span><span class="sxs-lookup"><span data-stu-id="c6a5a-102">VPN related issues</span></span>

<span data-ttu-id="c6a5a-103">Pomyślne wdrożenie łączności sieci VPN dla klientów MDM zależy od wdrożonego profilu, który poprawnie odzwierciedla wymagania infrastruktury sieci VPN.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="c6a5a-104">Aby uzyskać odpowiednie ustawienia dla platform klienckich, które badasz, zobacz:</span><span class="sxs-lookup"><span data-stu-id="c6a5a-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="c6a5a-105">Ustawienia urządzenia holograficznego systemu Windows 10 i systemu Windows w celu dodawania połączeń sieci VPN przy użyciu usługi Intune</span><span class="sxs-lookup"><span data-stu-id="c6a5a-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="c6a5a-106">Dodawanie ustawień sieci VPN na urządzeniach z systemem iOS i iPadOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c6a5a-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="c6a5a-107">Ustawienia urządzenia z systemem Android do konfigurowania sieci VPN w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="c6a5a-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="c6a5a-108">Dodawanie ustawień sieci VPN na urządzeniach z systemem macOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c6a5a-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="c6a5a-109">Jeśli profil sieci VPN używa uwierzytelniania opartego na certyfikatach, upewnij się, że profile certyfikatów głównych i certyfikatów uwierzytelniania klienta połączone z profilem sieci VPN zostały pomyślnie wdrożone.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="c6a5a-110">**Typowe problemy**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-110">**Common Issues**</span></span>

<span data-ttu-id="c6a5a-111">**Wdrożyłem profil sieci VPN na urządzeniu. Usługa Intune pokazuje, że zakończyło się pomyślnie, ale urządzenie nie łączy się z siecią VPN.**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="c6a5a-112">Pomyślny stan oznacza, że usługa Intune pomyślnie wdrożyła profil skonfigurowany.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="c6a5a-113">Jednak te konfiguracje mogą nie odpowiadać wymaganiom sieci i/lub uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="c6a5a-114">Przejrzyj dzienniki w usłudze infrastruktury i uwierzytelniania (na serwerze sieci VPN i serwerze NPS/Radius), aby uzyskać więcej informacji na temat próby połączenia.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="c6a5a-115">Może być konieczna praca z zespołem infrastruktury sieciowej lub dostawcą sieci VPN innej firmy w celu zbierania i przeglądania dzienników.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="c6a5a-116">**Po skonfigurowaniu niestandardowej sieci VPN dla systemu iOS funkcja sieci VPN dla aplikacji nie jest dostępna.**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="c6a5a-117">Sieć VPN dla aplikacji dla urządzeń z systemem iOS w usłudze Intune jest obecnie dostępna dla określonej listy dostawców i partnerów, którzy muszą również spełniać wymagania wstępne certyfikatu przed skonfigurowaniem sieci VPN dla poszczególnych aplikacji.</span><span class="sxs-lookup"><span data-stu-id="c6a5a-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="c6a5a-118">Aby uzyskać więcej informacji, zobacz [Konfigurowanie wirtualnej sieci prywatnej (VPN) dla urządzeń z systemem iOS/iPadOS dla aplikacji w usłudze Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="c6a5a-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="c6a5a-119">Aby uzyskać więcej informacji o wszystkich typach połączeń sieci VPN w usłudze Intune, zobacz Tworzenie profilów sieci VPN w [celu nawiązania połączenia z serwerami sieci VPN w usłudze Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="c6a5a-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="c6a5a-120">**Sieć VPN na żądanie systemu iOS nie jest wyzwalana, gdy jest dostępna skonfigurowana domena**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="c6a5a-121">Aby przetestować automatyczne ustawienia sieci VPN, ustaw następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="c6a5a-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="c6a5a-122">Chcę wykonać następujące czynności: **Oceń każdą próbę połączenia**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="c6a5a-123">Wybierz, czy chcesz się połączyć: **W razie potrzeby połącz się**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="c6a5a-124">Gdy użytkownicy uzyskują dostęp do tych domen: **docelowa** *nazwa domeny*</span><span class="sxs-lookup"><span data-stu-id="c6a5a-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="c6a5a-125">Jeśli powyższa konfiguracja nie powiedzie się, dodaj następujący element:</span><span class="sxs-lookup"><span data-stu-id="c6a5a-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="c6a5a-126">Gdy ten adres URL jest nieosiągalny, wymuś połączenie sieci VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="c6a5a-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>