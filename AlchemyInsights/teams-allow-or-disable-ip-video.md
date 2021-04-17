---
title: Zespoły zezwalają na wideo IP lub wyłączą je
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826353"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="abf7a-102">Zespoły zezwalają na wideo IP lub wyłączą je</span><span class="sxs-lookup"><span data-stu-id="abf7a-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="abf7a-103">**Zmienianie lub tworzenie zasad spotkania**</span><span class="sxs-lookup"><span data-stu-id="abf7a-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="abf7a-104">Aby zmienić lub utworzyć zasady spotkania, przejdź do centrum administracyjnego usługi Microsoft Teams i > **spotkania > zasady spotkania.**</span><span class="sxs-lookup"><span data-stu-id="abf7a-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="abf7a-105">Wybierz zasadę z listy i kliknij **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="abf7a-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="abf7a-106">Jeśli tworzysz nową zasadę, dodaj nazwę i opis.</span><span class="sxs-lookup"><span data-stu-id="abf7a-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="abf7a-107">Nazwa nie może zawierać znaków specjalnych ani być dłuższa niż 64 znaki.</span><span class="sxs-lookup"><span data-stu-id="abf7a-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="abf7a-108">Wybierz odpowiednie ustawienia, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="abf7a-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="abf7a-109">Załóżmy na przykład, że masz wielu użytkowników i chcesz ograniczyć przepustowość, jaką będzie wymagało ich spotkanie.</span><span class="sxs-lookup"><span data-stu-id="abf7a-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="abf7a-110">W takim przypadku należy utworzyć nową zasadę niestandardową o nazwie „Ograniczona przepustowość” i wyłączyć następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="abf7a-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="abf7a-111">W sekcji **Dźwięk i wideo**:</span><span class="sxs-lookup"><span data-stu-id="abf7a-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="abf7a-112">wyłącz opcję Zezwalaj na nagrywanie w chmurze;</span><span class="sxs-lookup"><span data-stu-id="abf7a-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="abf7a-113">wyłącz opcję Zezwalaj na IP wideo.</span><span class="sxs-lookup"><span data-stu-id="abf7a-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="abf7a-114">Następnie przypisz tę zasadę do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="abf7a-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="abf7a-115">**Przypisywanie użytkownikom zasady dotyczącej spotkania**</span><span class="sxs-lookup"><span data-stu-id="abf7a-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="abf7a-116">W lewej części obszaru nawigacji centrum administracyjnego usługi Microsoft Teams przejdź do pozycji **Użytkownicy**, a następnie kliknij użytkownika.</span><span class="sxs-lookup"><span data-stu-id="abf7a-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="abf7a-117">Kliknij z lewej strony nazwy użytkownika, aby go zaznaczyć, a następnie kliknij pozycję **Edytuj ustawienia**.</span><span class="sxs-lookup"><span data-stu-id="abf7a-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="abf7a-118">W **obszarze Zasady** spotkania wybierz zasady, które chcesz przypisać, a następnie kliknij przycisk **Zastosuj**.</span><span class="sxs-lookup"><span data-stu-id="abf7a-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="abf7a-119">Aby uzyskać więcej informacji, zobacz [Zarządzanie zasadami spotkań w aplikacji Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="abf7a-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
