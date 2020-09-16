---
title: Aplikacja Teams umożliwia lub wyłącza wideo IP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670194"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="7d4f7-102">Aplikacja Teams umożliwia lub wyłącza wideo IP</span><span class="sxs-lookup"><span data-stu-id="7d4f7-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="7d4f7-103">**Zmienianie lub tworzenie zasad dotyczących spotkania**</span><span class="sxs-lookup"><span data-stu-id="7d4f7-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="7d4f7-104">Aby zmienić lub utworzyć zasady dotyczące spotkania, przejdź do **Centrum administracyjnego usługi Microsoft teams > spotkań > zasad spotkania**.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="7d4f7-105">Wybierz zasadę z listy i kliknij **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="7d4f7-106">Jeśli tworzysz nową zasadę, dodaj nazwę i opis.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="7d4f7-107">Nazwa nie może zawierać znaków specjalnych ani być dłuższa niż 64 znaki.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="7d4f7-108">Wybierz odpowiednie ustawienia, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="7d4f7-109">Załóżmy na przykład, że masz wielu użytkowników i chcesz ograniczyć przepustowość, jaką będzie wymagała spotkania.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="7d4f7-110">W takim przypadku należy utworzyć nową zasadę niestandardową o nazwie „Ograniczona przepustowość” i wyłączyć następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="7d4f7-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="7d4f7-111">W sekcji **Dźwięk i wideo**:</span><span class="sxs-lookup"><span data-stu-id="7d4f7-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="7d4f7-112">wyłącz opcję Zezwalaj na nagrywanie w chmurze;</span><span class="sxs-lookup"><span data-stu-id="7d4f7-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="7d4f7-113">wyłącz opcję Zezwalaj na IP wideo.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="7d4f7-114">Następnie przypisz tę zasadę do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="7d4f7-115">**Przypisywanie użytkownikom zasady dotyczącej spotkania**</span><span class="sxs-lookup"><span data-stu-id="7d4f7-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="7d4f7-116">W lewej części obszaru nawigacji centrum administracyjnego usługi Microsoft Teams przejdź do pozycji **Użytkownicy**, a następnie kliknij użytkownika.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="7d4f7-117">Kliknij z lewej strony nazwy użytkownika, aby go zaznaczyć, a następnie kliknij pozycję **Edytuj ustawienia**.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="7d4f7-118">W obszarze **zasady spotkania**wybierz zasady, które chcesz przypisać, a następnie kliknij przycisk **Zastosuj**.</span><span class="sxs-lookup"><span data-stu-id="7d4f7-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="7d4f7-119">Aby uzyskać więcej informacji, zobacz [Zarządzanie zasadami dotyczącymi spotkań w aplikacji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="7d4f7-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
