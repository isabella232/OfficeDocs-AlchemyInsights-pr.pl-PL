---
title: Zarządzanie dostępem do sieci Web w przeglądarce Microsoft Edge dla systemów iOS i Android za pomocą usługi Microsoft Intune
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679603"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="6db23-102">Zarządzanie dostępem do sieci Web w przeglądarce Microsoft Edge dla systemów iOS i Android za pomocą usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6db23-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="6db23-103">Program Microsoft Edge dla systemów iOS i Android umożliwia użytkownikom przeglądanie sieci Web z wielu całkowicie oddzielonych profilów.</span><span class="sxs-lookup"><span data-stu-id="6db23-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="6db23-104">Dostęp do najszerszych możliwości ochrony danych programu Microsoft 365 jest dostępny po zasubskrybowaniu pakietu Enterprise Mobility + Security Suite, który obejmuje funkcje Microsoft Intune i usługi Azure Active Directory Premium, takie jak dostęp warunkowy.</span><span class="sxs-lookup"><span data-stu-id="6db23-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="6db23-105">W tym celu należy wdrożyć zasady dostępu warunkowego, które (1) umożliwiają użytkownikom nawiązywanie połączeń z urządzeń przenośnych z programem Microsoft Edge dla systemów iOS i Android oraz to (2) implementujące zasady ochrony aplikacji usługi Microsoft Intune zapewniające chronione środowisko przeglądania.</span><span class="sxs-lookup"><span data-stu-id="6db23-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="6db23-106">Aby zrozumieć, jak można korzystać z dostępu warunkowego i zasad, zobacz:</span><span class="sxs-lookup"><span data-stu-id="6db23-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="6db23-107">Stosowanie zasad dostępu warunkowego usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6db23-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="6db23-108">Tworzenie zasad ochrony aplikacji Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6db23-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="6db23-109">Korzystanie z logowania jednokrotnego w usłudze Azure Active Directory — połączone aplikacje sieci Web w przeglądarkach chronionych zasadami</span><span class="sxs-lookup"><span data-stu-id="6db23-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="6db23-110">Zarządzanie doświadczeniem w przeglądaniu za pomocą konfiguracji aplikacji</span><span class="sxs-lookup"><span data-stu-id="6db23-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="6db23-111">Zezwalanie na używanie tylko kont służbowych i szkolnych</span><span class="sxs-lookup"><span data-stu-id="6db23-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="6db23-112">Wdrażanie ogólnych zasad konfiguracji aplikacji</span><span class="sxs-lookup"><span data-stu-id="6db23-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="6db23-113">Wdrażanie zasad konfiguracji aplikacji na potrzeby ochrony danych</span><span class="sxs-lookup"><span data-stu-id="6db23-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="6db23-114">Wdrażanie zasad konfiguracji aplikacji za pomocą programu Microsoft Endpoint Manager</span><span class="sxs-lookup"><span data-stu-id="6db23-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="6db23-115">Aby dowiedzieć się, jak uzyskać dostęp do zarządzanych dzienników aplikacji, zobacz [Korzystanie z przeglądarki Microsoft Edge dla systemów iOS i Android w celu uzyskiwania dostępu do dzienników aplikacji zarządzanych](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="6db23-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
