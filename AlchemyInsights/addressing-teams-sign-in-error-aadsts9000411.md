---
title: Adresowanie błędu logowania do zespołów AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821997"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="1ca1b-102">Adresowanie błędu logowania do zespołów AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="1ca1b-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="1ca1b-103">Podczas logowania się do aplikacji Microsoft Teams może zostać wyświetlony komunikat o błędzie: Niestety, ale mamy problem z zalogowaniem Cię do **AADSTS9000411: Żądanie nie jest poprawnie sformatowane. Parametr "login_hint" został zduplikowany.**</span><span class="sxs-lookup"><span data-stu-id="1ca1b-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="1ca1b-104">Aby rozwiązać ten problem, upewnij się, że Twoi klienci aplikacji Microsoft Teams są zaktualizowani.</span><span class="sxs-lookup"><span data-stu-id="1ca1b-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="1ca1b-105">Aby uzyskać więcej informacji na temat aktualizowania klienta, zobacz [Aktualizowanie aplikacji Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="1ca1b-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="1ca1b-106">Jeśli z jakiegoś powodu nie możesz zaktualizować klienta, wylogowanie się z klienta spowoduje wyczyszczenie większości danych buforowanych.</span><span class="sxs-lookup"><span data-stu-id="1ca1b-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="1ca1b-107">Jeśli jednak po zalogowaniu/zalogowaniu nadal masz problemy, zamknij usługę Teams i wyczyść pamięć podręczną klienta, wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="1ca1b-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="1ca1b-108">Zamknij usługę Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1ca1b-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="1ca1b-109">Przejdź do: %appdata%\microsoft\teams i usuń wszystkie pliki.</span><span class="sxs-lookup"><span data-stu-id="1ca1b-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="1ca1b-110">Otwórz ponownie usługę Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1ca1b-110">Reopen Microsoft Teams.</span></span>
