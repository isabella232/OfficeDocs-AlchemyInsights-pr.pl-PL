---
title: Automatyczne logowanie się do programu Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398739"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="5bbec-102">Automatyczne logowanie się do programu Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="5bbec-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="5bbec-103">Program Microsoft Edge używa domyślnego konta systemu operacyjnego do automatycznego logowania użytkownika zgodnie z konfiguracją urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="5bbec-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="5bbec-104">Poniżej opisano scenariusze dotyczące poszczególnych typów konfiguracji urządzenia i zależnego od niego procesu logowania użytkownika:</span><span class="sxs-lookup"><span data-stu-id="5bbec-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="5bbec-105">**To urządzenie jest hybrydowe/AAD-J:** Ta opcja jest dostępna w systemie Windows 10 oraz w odpowiednich wersjach serwera.</span><span class="sxs-lookup"><span data-stu-id="5bbec-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="5bbec-106">Użytkownicy są automatycznie zalogowani przy użyciu kont usługi Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="5bbec-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="5bbec-107">**Urządzenie jest przyłączone do** domeny: Ta opcja jest dostępna w systemie Windows 10, na poziomie poprzednich wersji systemu Windows i w odpowiadających im wersjach serwera.</span><span class="sxs-lookup"><span data-stu-id="5bbec-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="5bbec-108">Domyślnie użytkownicy z kontami domeny nie są zalogowani automatycznie. aby włączyć dla nich automatyczne logowanie się, użyj zasad **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="5bbec-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="5bbec-109">Aby włączyć automatyczne logowanie dla użytkowników z kontami usługi Azure AD, rozważ dołączanie hybrydowe ich urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5bbec-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="5bbec-110">Konto domyślne systemu operacyjnego to konto **Microsoft:** Ta opcja jest dostępna w systemie Windows 10 RS3 (wersja 1709, kompilacja 10.0.16299) i w nowszych wersjach.</span><span class="sxs-lookup"><span data-stu-id="5bbec-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="5bbec-111">Scenariusz jest mało prawdopodobny na urządzeniach w przedsiębiorstwie.</span><span class="sxs-lookup"><span data-stu-id="5bbec-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="5bbec-112">Jeśli jednak kontem domyślnym systemu operacyjnego jest konto Microsoft, program Microsoft Edge automatycznie zaloguje się użytkownika za pomocą konta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5bbec-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
