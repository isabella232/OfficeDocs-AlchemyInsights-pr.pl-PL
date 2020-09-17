---
title: Dwukrotne kliknięcie pliku pakietu Office nie powoduje otwarcia go
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812089"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="78a4f-102">Dwukrotne kliknięcie pliku pakietu Office nie powoduje otwarcia go</span><span class="sxs-lookup"><span data-stu-id="78a4f-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="78a4f-103">Po dwukrotnym kliknięciu pliku pakietu Office może zostać wyświetlony program otwarty, ale sam plik nie jest otwierany.</span><span class="sxs-lookup"><span data-stu-id="78a4f-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="78a4f-104">Może też zostać wyświetlony komunikat o błędzie: "Wystąpił problem podczas wysyłania polecenia do programu".</span><span class="sxs-lookup"><span data-stu-id="78a4f-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="78a4f-105">Istnieje wiele powodów tego problemu, ale dwa najczęstsze rozwiązania to:</span><span class="sxs-lookup"><span data-stu-id="78a4f-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="78a4f-106">W programie Excel upewnij się, że opcja DDE nie jest zaznaczona.</span><span class="sxs-lookup"><span data-stu-id="78a4f-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="78a4f-107">Tę opcję można znaleźć, tworząc nowy skoroszyt, a następnie wybierając pozycję **opcje > plików > zaawansowane**.</span><span class="sxs-lookup"><span data-stu-id="78a4f-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="78a4f-108">W sekcji **Ogólne** Usuń zaznaczenie pola wyboru **Ignoruj inne aplikacje korzystające z dynamicznej wymiany danych (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="78a4f-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="78a4f-109">Uruchom naprawę online, aby przywrócić ustawienia domyślne.</span><span class="sxs-lookup"><span data-stu-id="78a4f-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="78a4f-110">Kliknij przycisk Start systemu Windows i wyszukaj ciąg "Panel sterowania".</span><span class="sxs-lookup"><span data-stu-id="78a4f-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="78a4f-111">Otwórz **Panel sterowania**i przejdź do **apletu programy > programy i funkcje**.</span><span class="sxs-lookup"><span data-stu-id="78a4f-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="78a4f-112">Następnie kliknij prawym przyciskiem myszy pozycję **Microsoft Office [Version]** i wybierz polecenie **Zmień > naprawy online**.</span><span class="sxs-lookup"><span data-stu-id="78a4f-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="78a4f-113">Jeśli żadne z tych rozwiązań nie działa, można znaleźć bardziej kompletną listę rozwiązań w artykule pomocy technicznej, [klikając dwukrotnie plik pakietu Office nie może go otworzyć](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="78a4f-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
