---
title: Automatyczne logowanie w przeglądarce Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678811"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="8f04b-102">Automatyczne logowanie w przeglądarce Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="8f04b-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="8f04b-103">Program Microsoft Edge używa domyślnego konta systemu operacyjnego do automatycznego logowania użytkownika zgodnie z konfiguracją urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="8f04b-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="8f04b-104">Poniżej opisano scenariusze poszczególnych typów konfiguracji urządzeń oraz proces logowania się do niego zależne.</span><span class="sxs-lookup"><span data-stu-id="8f04b-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="8f04b-105">To **urządzenie jest hybrydowe/AAD-J**: Ta opcja jest dostępna w systemie Windows 10, w systemie Windows, na poziomie niższego poziomu i w odpowiednich wersjach serwera.</span><span class="sxs-lookup"><span data-stu-id="8f04b-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8f04b-106">Użytkownicy są automatycznie logowani przy użyciu kont usługi Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="8f04b-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="8f04b-107">**Urządzenie jest przyłączone do domeny**: Ta opcja jest dostępna w systemie Windows 10, na poziomie systemu Windows i w odpowiednich wersjach serwera.</span><span class="sxs-lookup"><span data-stu-id="8f04b-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8f04b-108">Domyślnie użytkownicy z kontami domeny nie są zalogowani automatycznie; Aby włączyć automatyczne logowanie, użyj zasad **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="8f04b-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="8f04b-109">Aby włączyć automatyczne logowanie użytkowników z kontami usługi Azure AD, weź pod ³ ¹ łączenie hybrydowe urządzeń.</span><span class="sxs-lookup"><span data-stu-id="8f04b-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="8f04b-110">**Domyślne konto systemu operacyjnego to konto Microsoft**: Ta opcja jest dostępna w systemie Windows 10 RS3 (wersja 1709, Kompilacja 10.0.16299) i w nowszych wersjach.</span><span class="sxs-lookup"><span data-stu-id="8f04b-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="8f04b-111">W przypadku urządzeń z jednostkami biznesowymi nie ma mało prawdopodobnego scenariusza.</span><span class="sxs-lookup"><span data-stu-id="8f04b-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="8f04b-112">Jeśli jednak domyślnym kontem systemu operacyjnego jest konto Microsoft, program Microsoft Edge automatycznie zaloguje użytkownika przy użyciu konta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8f04b-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
