---
title: Tworzenie zasad i profilów usługi Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704652"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="f7dcf-102">Tworzenie zasad i profilów usługi Intune</span><span class="sxs-lookup"><span data-stu-id="f7dcf-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="f7dcf-103">W usłudze Intune możesz tworzyć zasady i profile, które mają różne funkcje.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="f7dcf-104">**Profile rejestracji:** wstępnie skonfiguruj urządzenia według platformy, włącz skojalność użytkowników, korzystaj z uwierzytelniania wieloskładnikowego i nie tylko.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="f7dcf-105">[Dobrymi zasobami są rejestrowanie](https://docs.microsoft.com/intune/device-enrollment)urządzeń i tworzenie profilów rejestracji dla [systemów Android,](https://docs.microsoft.com/intune/android-enroll) [iOS,](https://docs.microsoft.com/intune/ios-enroll) [macOS](https://docs.microsoft.com/intune/macos-enroll)i [Windows.](https://docs.microsoft.com/intune/windows-enrollment-methods)</span><span class="sxs-lookup"><span data-stu-id="f7dcf-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="f7dcf-106">**Zasady zgodności:** zdefiniuj reguły i ustawienia, które muszą być zgodne przez urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="f7dcf-107">Za pomocą zasad zgodności można również monitorować urządzenia i powiadamiać użytkowników o niezgodnościach.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="f7dcf-108">Wprowadzenie do [zasad zgodności urządzeń.](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="f7dcf-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="f7dcf-109">**Zasady dostępu warunkowego:** ułatwiają zabezpieczanie zasobów organizacji w zależności od wprowadzanych warunków.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="f7dcf-110">Na przykład w przypadku urządzeń, które nie są zgodne, użyj dostępu warunkowego w celu ograniczenia dostępu do poczty e-mail i programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="f7dcf-111">[Co to jest dostęp warunkowy](https://docs.microsoft.com/intune/conditional-access) i typowe sposoby korzystania z dostępu [warunkowego](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) to dobre zasoby, aby rozpocząć pracę.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="f7dcf-112">**Profile konfiguracji:** zarządzaj funkcjami i ustawieniami na urządzeniach, w tym ustawieniami poczty e-mail, dodaj sieć Wi-Fi, korzystaj z wbudowanych szablonów, kontroluj funkcje urządzeń z systemami iOS i macOS i nie tylko.</span><span class="sxs-lookup"><span data-stu-id="f7dcf-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="f7dcf-113">Rozpoczynanie pracy w [profilach konfiguracji urządzenia.](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="f7dcf-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="f7dcf-114">Przydatne linki:</span><span class="sxs-lookup"><span data-stu-id="f7dcf-114">Helpful links:</span></span>

- [<span data-ttu-id="f7dcf-115">Typowe pytania, problemy i rozwiązania dotyczące zasad i profilów urządzeń w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="f7dcf-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="f7dcf-116">Rozwiązywanie problemów z zasadami i profilami w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="f7dcf-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
