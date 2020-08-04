---
title: Profile sieci Wi-Fi usługi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555316"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="e8710-102">Profile sieci Wi-Fi usługi Intune</span><span class="sxs-lookup"><span data-stu-id="e8710-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="e8710-103">Pomyślne wdrożenie łączności Wi-Fi dla klientów MDM zależy od poprawnie wdrożonego profilu, który odzwierciedla wymagania firmowej infrastruktury Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e8710-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="e8710-104">Aby przejrzeć odpowiednie ustawienia dla analizowych platform klienckich, zobacz:</span><span class="sxs-lookup"><span data-stu-id="e8710-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="e8710-105">Dodawanie ustawień sieci Wi-Fi dla urządzeń z systemem Android w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e8710-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="e8710-106">Dodawanie ustawień sieci Wi-Fi dla urządzeń dedykowanych i w pełni zarządzanych systemu Android Enterprise w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e8710-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="e8710-107">Dodawanie ustawień sieci Wi-Fi dla urządzeń z systemem iOS i iPadOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e8710-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="e8710-108">Dodawanie ustawień sieci Wi-Fi dla urządzeń z systemem Windows 10 i nowszych w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="e8710-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="e8710-109">Importowanie ustawień sieci Wi-Fi dla urządzeń z systemem Windows w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="e8710-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="e8710-110">**Typowe problemy**</span><span class="sxs-lookup"><span data-stu-id="e8710-110">**Common Issues**</span></span>

<span data-ttu-id="e8710-111">**Wdrażam profil sieci Wi-Fi zależny od wdrożonego certyfikatu określonego w profilu sieci Wi-Fi. Jednak profile konfiguracji są wyświetlane stan błędu.**</span><span class="sxs-lookup"><span data-stu-id="e8710-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="e8710-112">Sprawdź, czy urządzenie odebrało certyfikat.</span><span class="sxs-lookup"><span data-stu-id="e8710-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="e8710-113">W usłudze Intune przejdź do **opcji Wszystkie urządzenia** i wybierz **konfigurację urządzenia**> urządzenia .</span><span class="sxs-lookup"><span data-stu-id="e8710-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="e8710-114">Sprawdź, czy wszystkie oczekiwane profile są wymienione i w stanie pomyślnym.</span><span class="sxs-lookup"><span data-stu-id="e8710-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="e8710-115">W przypadku profilu systemu Android, jeśli masz certyfikaty pośrednie w łańcuchu certyfikatów, upewnij się, że są one wdrażane na urządzeniach z systemem Android.</span><span class="sxs-lookup"><span data-stu-id="e8710-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="e8710-116">Aby sprawdzić stan certyfikatu, przejdź do **profili konfiguracji urządzenia**Android pośredni certyfikat urzędu  >  **Profiles**  >  **Android intermediate CA**  >  **certyfikacji.**  >  **Trusted Certificate**</span><span class="sxs-lookup"><span data-stu-id="e8710-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="e8710-117">Jeśli nadal widzisz błędy, przejrzyj procedury i sekcje rozwiązywania problemów.</span><span class="sxs-lookup"><span data-stu-id="e8710-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="e8710-118">Aby uzyskać więcej informacji, zobacz [Omówienie rozwiązywania problemów z profilami certyfikatów SCEP za pomocą usługi Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e8710-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="e8710-119">**Wdrożeniu profilu sieci Wi-Fi na urządzeniu. Usługa Intune pokazuje, że zakończyła się pomyślnie, ale urządzenie nie łączy się z siecią Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="e8710-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="e8710-120">Pomyślny stan oznacza, że usługa Intune pomyślnie wdrożyła profil skonfigurowany.</span><span class="sxs-lookup"><span data-stu-id="e8710-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="e8710-121">Jednak te konfiguracje mogą nie odpowiadać wymaganiom sieci i/lub uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="e8710-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="e8710-122">Aby uzyskać więcej informacji na temat próby połączenia, przejrzyj dzienniki w usłudze infrastruktury i uwierzytelniania (na kontrolerze punktu dostępu Wi-Fi i serwerze NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="e8710-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="e8710-123">Może być nawiązywać współpraca z zespołem infrastruktury sieciowej lub dostawcą sieci Wi-Fi innej firmy w celu zbierania i przeglądania dzienników.</span><span class="sxs-lookup"><span data-stu-id="e8710-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>