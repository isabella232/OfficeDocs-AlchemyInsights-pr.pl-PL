---
title: Wdrażanie programu Microsoft Edge w systemach iOS, iPadOS i Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194516"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="2d519-102">Wdrażanie programu Microsoft Edge w systemach iOS, iPadOS i Android</span><span class="sxs-lookup"><span data-stu-id="2d519-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="2d519-103">Poniższy scenariusz z przewodnikiem pomoże Ci przypisać program Microsoft Edge użytkownikom urządzeń z systemami iOS, iPadOS i Android.</span><span class="sxs-lookup"><span data-stu-id="2d519-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="2d519-104">Jeśli zablokowano użytkownikom rejestrowanie urządzeń przenośnych, ten scenariusz z przewodnikiem nie będzie działać i użytkownicy będą musieli zainstalować program Microsoft Edge samodzielnie.</span><span class="sxs-lookup"><span data-stu-id="2d519-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="2d519-105">Scenariusz z przewodnikiem obejmuje następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="2d519-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="2d519-106">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="2d519-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="2d519-107">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="2d519-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="2d519-108">Podstawy</span><span class="sxs-lookup"><span data-stu-id="2d519-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="2d519-109">Konfiguracja</span><span class="sxs-lookup"><span data-stu-id="2d519-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="2d519-110">Zadania</span><span class="sxs-lookup"><span data-stu-id="2d519-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="2d519-111">Recenzja i tworzenie</span><span class="sxs-lookup"><span data-stu-id="2d519-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="2d519-112">Po zakończeniu kroków w scenariuszu z przewodnikiem zasady usługi Microsoft Intune włączą następujące funkcje programu Microsoft Edge dla firm:</span><span class="sxs-lookup"><span data-stu-id="2d519-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="2d519-113">Tożsamość dwurdzeniowa</span><span class="sxs-lookup"><span data-stu-id="2d519-113">Dual identity</span></span>
- <span data-ttu-id="2d519-114">Integracja z zasadami ochrony aplikacji usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d519-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="2d519-115">Integracja z serwerem proxy aplikacji Usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2d519-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="2d519-116">Zarządzane ulubione i skróty strony głównej</span><span class="sxs-lookup"><span data-stu-id="2d519-116">Managed favorites and home page shortcuts</span></span>
