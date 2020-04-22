---
title: Rozwiązywanie problemów — nie znaleziono użytkownika w katalogu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702748"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="470b0-102">Rozwiązywanie problemów — nie znaleziono użytkownika w katalogu</span><span class="sxs-lookup"><span data-stu-id="470b0-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="470b0-103">Jeśli użytkownicy otrzymują komunikat o błędzie "nie można znaleźć użytkownika" w katalogu, spróbuj ponownie, gdzie typ problemu jest użytkownik nie w katalogu.</span><span class="sxs-lookup"><span data-stu-id="470b0-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="470b0-104">Poniższe kroki można wykonać, aby rozwiązać problem.</span><span class="sxs-lookup"><span data-stu-id="470b0-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="470b0-105">Upewnij się, że konto, które zaakceptowało zaproszenie e-mail, jest tym samym kontem, które jest używane do późniejszego logowania.</span><span class="sxs-lookup"><span data-stu-id="470b0-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="470b0-106">Upewnij się, że użytkownik używa tego samego konta, aby zaakceptować zaproszenie i zalogować się do witryny.</span><span class="sxs-lookup"><span data-stu-id="470b0-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="470b0-107">Aby uzyskać więcej informacji, zobacz [Jak zarządzać</a> aliasami dla konta Microsoft, aby zarządzać loginem usługi Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="470b0-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="470b0-108">Przejdź do każdej witryny, w której użytkownik otrzymuje błąd.</span><span class="sxs-lookup"><span data-stu-id="470b0-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="470b0-109">Dodaj "/_layouts/15/people.aspx/membershipgroupid=0" (w cudzysłowach) na końcu adresu URL witryny.</span><span class="sxs-lookup"><span data-stu-id="470b0-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="470b0-110">Przykład: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="470b0-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="470b0-111">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="470b0-111">Select the user from the list.</span></span>

- <span data-ttu-id="470b0-112">Kliknij pozycję **Usuń uprawnienia użytkownika** ze Wstążki.</span><span class="sxs-lookup"><span data-stu-id="470b0-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="470b0-113">Dodaj ponownie użytkownika i ponownie syłkuj zaproszenie do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="470b0-113">Add back the User and Resend the invite to the user.</span></span>

