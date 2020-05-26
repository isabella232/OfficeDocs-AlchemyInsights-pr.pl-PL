---
title: Błąd logowania zespołów adresowania AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357874"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="c1194-102">Błąd logowania zespołów adresowania AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="c1194-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="c1194-103">Podczas logowania się do usługi Microsoft Teams może pojawić się błąd: **Przepraszamy, ale mamy problemy z podpisywaniem Cię w Usłudze AADSTS9000411: Żądanie nie jest poprawnie sformatowane. Parametr "login_hint" jest duplikowany.**</span><span class="sxs-lookup"><span data-stu-id="c1194-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="c1194-104">Aby rozwiązać ten problem, upewnij się, że klienci usługi Microsoft Teams są aktualizowani.</span><span class="sxs-lookup"><span data-stu-id="c1194-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="c1194-105">Aby uzyskać więcej informacji na temat aktualizowania klienta, zobacz [Aktualizowanie usługi Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="c1194-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="c1194-106">Jeśli nie można zaktualizować klienta z jakiegoś powodu, wylogowanie klienta spowoduje wyczyszczenie większości danych w pamięci podręcznej.</span><span class="sxs-lookup"><span data-stu-id="c1194-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="c1194-107">Jeśli jednak nadal występują problemy po wylogowaniu/logowaniu, zamknij program Teams i wyczyść pamięć podręczną klienta, wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="c1194-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="c1194-108">Zamknij usługi Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c1194-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="c1194-109">Przejdź do: %appdata%\microsoft\teams i usuń wszystkie pliki.</span><span class="sxs-lookup"><span data-stu-id="c1194-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="c1194-110">Ponowne otwarcie usługi Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c1194-110">Reopen Microsoft Teams.</span></span>
