---
title: Nie można otworzyć dwukrotnego kliknięcia pliku pakietu Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814815"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="5c967-102">Nie można otworzyć dwukrotnego kliknięcia pliku pakietu Office</span><span class="sxs-lookup"><span data-stu-id="5c967-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="5c967-103">Po dwukrotnym kliknięciu pliku pakietu Office może zostać wyświetlony otwarty program, ale sam plik nie zostanie otwarty.</span><span class="sxs-lookup"><span data-stu-id="5c967-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="5c967-104">Może też zostać wyświetlany komunikat o błędzie: "Wystąpił problem podczas wysyłania polecenia do programu".</span><span class="sxs-lookup"><span data-stu-id="5c967-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="5c967-105">Przyczyn jest wiele, ale dwa najczęściej spotykane rozwiązania są takie:</span><span class="sxs-lookup"><span data-stu-id="5c967-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="5c967-106">W programie Excel upewnij się, że opcja DDE nie jest zaznaczona.</span><span class="sxs-lookup"><span data-stu-id="5c967-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="5c967-107">Tę opcję można znaleźć, tworząc nowy skoroszyt, a następnie wybierając pozycję Plik **> opcje > zaawansowane.**</span><span class="sxs-lookup"><span data-stu-id="5c967-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="5c967-108">W sekcji **Ogólne** wyczyść pole wyboru Ignoruj inne aplikacje, które korzystają z dynamicznej wymiany danych **(DDE, Dynamic Data Exchange).**</span><span class="sxs-lookup"><span data-stu-id="5c967-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="5c967-109">Uruchom naprawę online, aby przywrócić ustawienia domyślne.</span><span class="sxs-lookup"><span data-stu-id="5c967-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="5c967-110">Kliknij przycisk Start systemu Windows i wyszukaj pozycję "Panel sterowania".</span><span class="sxs-lookup"><span data-stu-id="5c967-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="5c967-111">Otwórz Panel **sterowania**, a następnie przejdź do **a programs > Programs and Features**.</span><span class="sxs-lookup"><span data-stu-id="5c967-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="5c967-112">Następnie kliknij prawym przyciskiem myszy **pozycję Microsoft Office [Wersja]** i wybierz pozycję **Zmień > Naprawa online.**</span><span class="sxs-lookup"><span data-stu-id="5c967-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="5c967-113">Jeśli żadne z tych rozwiązań nie działa, bardziej kompletną listę rozwiązań można znaleźć w artykule pomocy technicznej. Dwukrotne kliknięcie pliku pakietu Office nie powiedzie się, [aby go otworzyć.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="5c967-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
