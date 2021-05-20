---
title: Teams dla komputerów Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582080"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="95f85-102">Teams dla komputerów Mac</span><span class="sxs-lookup"><span data-stu-id="95f85-102">Teams add-in for Mac</span></span>

<span data-ttu-id="95f85-103">Aby rozwiązać problemy z brakującym Teams dla użytkowników systemu operacyjnego Mac, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="95f85-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="95f85-104">**Krok 1.** Jeśli masz hybrydowe Exchange lokalne (wymagane jest 2016 CU3 lub nowsze), użyj narzędzia Test-HMA.ps1, aby potwierdzić, że nowoczesne uwierzytelnianie hybrydowe jest poprawnie skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="95f85-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="95f85-105">Aby uzyskać więcej informacji, zobacz Konfigurowanie nowoczesnego uwierzytelniania na platformach [Outlook dla systemów iOS i Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="95f85-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="95f85-106">**Uwaga** Użyj formatu adresu UPN (na przykład [username@contoso.com](mailto:username@contoso.com)), a nie domena #D0 a nazwa_użytkownika.</span><span class="sxs-lookup"><span data-stu-id="95f85-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="95f85-107">Robisz to nawet w przypadku użytkowników, Exchange Online skrzynki pocztowe.</span><span class="sxs-lookup"><span data-stu-id="95f85-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="95f85-108">**Krok 2.** Niech użytkownik może przejść do **narzędzia**  >  **Konta...** w Outlook dla komputerów Mac, a następnie znajdź i wybierz konto.</span><span class="sxs-lookup"><span data-stu-id="95f85-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="95f85-109">Upewnij się, że wymieniona nazwa użytkownika ma format UPN (na [przykład username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="95f85-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="95f85-110">**Krok 3.** Upewnij się, że użytkownik jest licencjonowanym Microsoft Teams użytkownikiem.</span><span class="sxs-lookup"><span data-stu-id="95f85-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="95f85-111">Użytkownik musi korzystać z subskrypcji usługi Office 365 dla komputerów Mac w wersji produktu 16.24 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="95f85-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>