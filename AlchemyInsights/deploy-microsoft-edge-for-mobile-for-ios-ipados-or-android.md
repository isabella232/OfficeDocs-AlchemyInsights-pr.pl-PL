---
title: Wdrażanie aplikacji Microsoft Edge dla urządzeń przenośnych w systemie iOS/iPadOS lub Android
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
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679939"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="12fa5-102">Wdrażanie aplikacji Microsoft Edge dla urządzeń przenośnych w systemie iOS/iPadOS lub Android</span><span class="sxs-lookup"><span data-stu-id="12fa5-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="12fa5-103">W poniższym scenariuszu przedstawionym poniżej przedstawiono sposób przypisywania przeglądarki Microsoft Edge do użytkowników urządzeń z systemem iOS, iPadOS i Android.</span><span class="sxs-lookup"><span data-stu-id="12fa5-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="12fa5-104">Po wykonaniu tych kroków zasady usługi Microsoft Intune będą umożliwiały Włączanie następujących funkcji przeglądarki Microsoft Edge dla firm:</span><span class="sxs-lookup"><span data-stu-id="12fa5-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="12fa5-105">Podwójna tożsamość</span><span class="sxs-lookup"><span data-stu-id="12fa5-105">Dual identity</span></span>
- <span data-ttu-id="12fa5-106">Integracja z zasadami ochrony aplikacji usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="12fa5-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="12fa5-107">Integracja z serwerem proxy aplikacji usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="12fa5-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="12fa5-108">Skróty do zarządzanych ulubionych i stron głównych</span><span class="sxs-lookup"><span data-stu-id="12fa5-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="12fa5-109">Jeśli zablokowano użytkownikom możliwość rejestrowania urządzeń przenośnych, ten scenariusz z przewodnikiem nie będzie działać, a użytkownicy będą musieli zainstalować przeglądarkę Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="12fa5-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="12fa5-110">Aby wdrożyć aplikację Microsoft Edge dla urządzeń przenośnych dla systemu iOS/iPadOS lub Android, zobacz:</span><span class="sxs-lookup"><span data-stu-id="12fa5-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="12fa5-111">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="12fa5-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="12fa5-112">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="12fa5-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="12fa5-113">Kwestie</span><span class="sxs-lookup"><span data-stu-id="12fa5-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="12fa5-114">Skonfigurowan</span><span class="sxs-lookup"><span data-stu-id="12fa5-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="12fa5-115">Pisania</span><span class="sxs-lookup"><span data-stu-id="12fa5-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="12fa5-116">Recenzja i tworzenie</span><span class="sxs-lookup"><span data-stu-id="12fa5-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
