---
title: Rozwiązywanie problemu - nie można odnaleźć w katalogu użytkownika
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544873"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="86896-102">Rozwiązywanie problemu - nie można odnaleźć w katalogu użytkownika</span><span class="sxs-lookup"><span data-stu-id="86896-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="86896-103">Jeśli użytkownicy otrzymują błąd komunikat "nie można znaleźć użytkownika" w katalogu.</span><span class="sxs-lookup"><span data-stu-id="86896-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="86896-104">Spróbuj ponownie gdzie typ problemu użytkownika nie jest w katalogu.</span><span class="sxs-lookup"><span data-stu-id="86896-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="86896-105">Następujące czynności mogą być wykonywane w celu rozwiązania problemu.</span><span class="sxs-lookup"><span data-stu-id="86896-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="86896-106">Upewnij się, konto, na którym przyjęte wiadomości e-mail z zaproszeniem jest to samo konto, który jest używany do logowania się później.</span><span class="sxs-lookup"><span data-stu-id="86896-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="86896-107">Upewnij się, że użytkownik korzysta z tego samego konta aby zaakceptować zaproszenie i zalogować się do witryny.</span><span class="sxs-lookup"><span data-stu-id="86896-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="86896-108">Aby uzyskać więcej informacji, zobacz [sposobu zarządzania aliasy konta Microsoft</a> do zarządzania logowania usługi Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="86896-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="86896-109">Przejdź do każdej witryny, w której użytkownik odbiera błąd.</span><span class="sxs-lookup"><span data-stu-id="86896-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="86896-110">Dodać "/ _layouts/15/people.aspx/membershipgroupid=0" (ujęty w cudzysłów podwójny) na końcu adresu URL witryny.</span><span class="sxs-lookup"><span data-stu-id="86896-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="86896-111">Przykład: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="86896-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="86896-112">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="86896-112">Select the user from the list.</span></span>

- <span data-ttu-id="86896-113">Kliknij przycisk **Usuń uprawnienia użytkownika** na Wstążce.</span><span class="sxs-lookup"><span data-stu-id="86896-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="86896-114">Dodać z powrotem użytkownika i ponownie wysłać zaproszenia do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="86896-114">Add back the User and Resend the invite to the user.</span></span>

