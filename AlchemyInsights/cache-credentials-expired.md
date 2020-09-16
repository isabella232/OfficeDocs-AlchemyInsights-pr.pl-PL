---
title: 'Błąd: nie można przekazać ani pobrać zmian, ponieważ poświadczenia w pamięci podręcznej wygasły'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734489"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="b2226-102">Błąd: nie można przekazać ani pobrać zmian, ponieważ poświadczenia w pamięci podręcznej wygasły</span><span class="sxs-lookup"><span data-stu-id="b2226-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="b2226-103">W przypadku zapisywania plików w aplikacji OneDrive, jeśli zostanie wyświetlony komunikat o błędzie zawierający frazę **"Twoje buforowane poświadczenia wygasły"**, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="b2226-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="b2226-104">Zamknij wszystkie aplikacje pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="b2226-104">Close all Office applications.</span></span>
1. <span data-ttu-id="b2226-105">Otwórz Menedżera poświadczeń i w polu wyszukiwania na pasku zadań wpisz nazwę **Menedżer poświadczeń** , a następnie wybierz pozycję **Panel sterowania Menedżera poświadczeń**.</span><span class="sxs-lookup"><span data-stu-id="b2226-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="b2226-106">Wybierz pozycję **poświadczenia systemu Windows**.</span><span class="sxs-lookup"><span data-stu-id="b2226-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="b2226-107">Znajdź dowolny wpis, który zaczyna się od aplikacji Word **OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="b2226-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="b2226-108">Zaznacz wpis, a następnie naciśnij klawisz **Remove**.</span><span class="sxs-lookup"><span data-stu-id="b2226-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="b2226-109">Zamknij Menedżera poświadczeń, a następnie kliknij prawym przyciskiem myszy niebieską chmurę w usłudze Systray, a następnie wybierz polecenie **Zamknij usługę OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="b2226-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="b2226-110">W polu wyszukiwania na pasku zadań wpisz **OneDrive** , a następnie wybierz pozycję **Aplikacja OneDrive** , aby uruchomić aplikację OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b2226-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="b2226-111">Zalogowanie się do usługi OneDrive, a następnie spróbuj zapisać plik w usłudze OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b2226-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
