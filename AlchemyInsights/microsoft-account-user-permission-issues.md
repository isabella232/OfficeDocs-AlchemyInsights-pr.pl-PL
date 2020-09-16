---
title: Rozwiązywanie problemu — nie znaleziono użytkownika w katalogu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725417"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="58602-102">Rozwiązywanie problemu — nie znaleziono użytkownika w katalogu</span><span class="sxs-lookup"><span data-stu-id="58602-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="58602-103">Jeśli użytkownicy otrzymują komunikat o błędzie "nie można odnaleźć użytkownika" w katalogu, spróbuj ponownie, gdzie typ problemu nie należy do katalogu.</span><span class="sxs-lookup"><span data-stu-id="58602-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="58602-104">Poniższe czynności można wykonać w celu rozwiązania problemu.</span><span class="sxs-lookup"><span data-stu-id="58602-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="58602-105">Upewnij się, że konto, które zaakceptował zaproszenie pocztą e-mail, jest tego samego konta, które jest używane do logowania się później.</span><span class="sxs-lookup"><span data-stu-id="58602-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="58602-106">Upewnij się, że użytkownik korzysta z tego samego konta w celu zaakceptowania zaproszenia i zarejestrowania się w witrynie.</span><span class="sxs-lookup"><span data-stu-id="58602-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="58602-107">Aby uzyskać więcej informacji, zobacz [jak zarządzać aliasami konta Microsoft, </a> Aby zarządzać logowaniem do usługi Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="58602-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="58602-108">Przejdź do każdej witryny, w której użytkownik otrzymuje błąd.</span><span class="sxs-lookup"><span data-stu-id="58602-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="58602-109">Dodaj "/_layouts/15/People.aspx/MembershipGroupId = 0" (w cudzysłowach podwójnych) na koniec adresu URL witryny.</span><span class="sxs-lookup"><span data-stu-id="58602-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="58602-110">Przykład: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="58602-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="58602-111">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="58602-111">Select the user from the list.</span></span>

- <span data-ttu-id="58602-112">Kliknij pozycję **Usuń uprawnienia użytkownika** na Wstążce.</span><span class="sxs-lookup"><span data-stu-id="58602-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="58602-113">Dodaj użytkownika i ponownie Wyślij zaproszenie do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="58602-113">Add back the User and Resend the invite to the user.</span></span>

