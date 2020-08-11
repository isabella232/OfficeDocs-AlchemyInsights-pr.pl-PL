---
title: Dodatek Teams dla komputerów Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629771"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="6657f-102">Dodatek Teams dla komputerów Mac</span><span class="sxs-lookup"><span data-stu-id="6657f-102">Teams add-in for Mac</span></span>

<span data-ttu-id="6657f-103">Aby rozwiązać problemy z brakującymi dodatkami dla użytkowników systemu operacyjnego dla komputerów Mac, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="6657f-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="6657f-104">**Krok 1.** Jeśli masz lokalnie lokalny program Exchange (2016 CU3 lub nowszy), użyj narzędzia Test-HMA.ps1, aby upewnić się, że nowoczesne uwierzytelnianie hybrydowe jest poprawnie skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="6657f-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="6657f-105">Aby uzyskać więcej informacji, zobacz [Sprawdzanie poprawności konfiguracji nowoczesnego uwierzytelniania dla aplikacji Outlook dla systemów iOS i Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="6657f-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="6657f-106">**Uwaga** Użyj formatu adresu UPN (na przykład [username@contoso.com](mailto:username@contoso.com)), a nie domena azwa_użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6657f-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="6657f-107">Zrób to nawet użytkownikom korzystającym ze skrzynek pocztowych usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6657f-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="6657f-108">**Krok 2.** Użytkownik powinien przejść do **narzędzi**  >  **konta**... w programie Outlook dla komputerów Mac, a następnie Znajdź i zaznacz konto.</span><span class="sxs-lookup"><span data-stu-id="6657f-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="6657f-109">Potwierdź, że nazwa użytkownika jest podana w formacie UPN (na przykład [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="6657f-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="6657f-110">**Krok 3:** Potwierdź, że użytkownik jest licencjonowanym użytkownikiem aplikacji Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6657f-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="6657f-111">Użytkownik musi korzystać z subskrypcji pakietu Office 365 dla komputerów Mac, produktu w wersji 16,24 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="6657f-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>