---
title: Nie można uzyskać dostępu do plików udostępnionych w czacie aplikacji Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51595819"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="fb26f-102">Nie można uzyskać dostępu do plików udostępnionych w czacie aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="fb26f-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="fb26f-103">W usłudze Microsoft Teams plik udostępniony przez użytkownika w oknie czatu jest automatycznie zapisywany w witrynie OneDrive użytkownika udostępniacego.</span><span class="sxs-lookup"><span data-stu-id="fb26f-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="fb26f-104">Gdy inny użytkownik spróbuje otworzyć plik w usłudze Teams i otrzymuje komunikat o błędzie "Nie masz dostępu do tego pliku", ten problem występuje, ponieważ w Twojej witrynie OneDrive aktywowano funkcję blokowania uprawnień użytkownika z ograniczonym dostępem.</span><span class="sxs-lookup"><span data-stu-id="fb26f-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="fb26f-105">Aby uzyskać instrukcje dotyczące wyłączania tej funkcji w witrynie usługi OneDrive, zobacz Błąd podczas [otwierania pliku w aplikacji Teams.](https://go.microsoft.com/fwlink/?linkid=2155733)</span><span class="sxs-lookup"><span data-stu-id="fb26f-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="fb26f-106">Sprawdź, czy inny użytkownik ma dostęp do witryny usługi OneDrive, i zapewnij do niego dostęp, zgodnie z instrukcjami w tece Udostępnianie plików [i folderów usługi OneDrive.](https://go.microsoft.com/fwlink/?linkid=2156017)</span><span class="sxs-lookup"><span data-stu-id="fb26f-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>