---
title: Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768811"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="78175-102">Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu</span><span class="sxs-lookup"><span data-stu-id="78175-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="78175-103">Jeśli użytkownicy otrzymują komunikat o błędzie "nie można znaleźć użytkownika" w katalogu, spróbuj ponownie, gdzie typ problemu jest użytkownik nie w katalogu.</span><span class="sxs-lookup"><span data-stu-id="78175-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="78175-104">Aby rozwiązać ten problem, można wykonać następujące czynności.</span><span class="sxs-lookup"><span data-stu-id="78175-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="78175-105">Upewnij się, że konto, które zaakceptował zaproszenie e-mail jest to samo konto, które jest używane do logowania się później.</span><span class="sxs-lookup"><span data-stu-id="78175-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="78175-106">Upewnij się, że użytkownik korzysta z tego samego konta, aby zaakceptować zaproszenie i zalogować się do witryny.</span><span class="sxs-lookup"><span data-stu-id="78175-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="78175-107">Aby uzyskać więcej informacji, zobacz [jak zarządzać aliasami konta</a> Microsoft w celu zarządzania biurem 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="78175-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="78175-108">Przejdź do każdej witryny, w którym użytkownik otrzymuje błąd.</span><span class="sxs-lookup"><span data-stu-id="78175-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="78175-109">Dodaj "/_layouts/15/People.aspx/MembershipGroupId = 0" (w cudzysłowie) na końcu adresu URL witryny.</span><span class="sxs-lookup"><span data-stu-id="78175-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="78175-110">Przykład: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="78175-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="78175-111">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="78175-111">Select the user from the list.</span></span>

- <span data-ttu-id="78175-112">Kliknij przycisk **Usuń uprawnienia użytkownika** ze wstążki.</span><span class="sxs-lookup"><span data-stu-id="78175-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="78175-113">Dodaj ponownie użytkownika i ponownie Wyślij zaproszenie do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="78175-113">Add back the User and Resend the invite to the user.</span></span>

