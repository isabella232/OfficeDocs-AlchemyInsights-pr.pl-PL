---
title: Rozwiązywanie problemów z awariami usługi OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749164"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="71ff5-102">Rozwiązywanie problemów z awariami usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="71ff5-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="71ff5-103">Jeśli usługa OneDrive wielokrotnie ulega awarii, spróbuj wykonać następujące kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="71ff5-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="71ff5-104">**Upewnij się, że klucze rejestru nie są ustawione:**</span><span class="sxs-lookup"><span data-stu-id="71ff5-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="71ff5-105">Korzystając z Edytora rejestru, przejdź do HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="71ff5-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="71ff5-106">Jeśli disableFileSyncNGSC jest obecny i ustawiony na 1, otwórz klucz i zmień wartość na 0.</span><span class="sxs-lookup"><span data-stu-id="71ff5-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="71ff5-107">Ręczne uruchamianie usługi OneDrive przez przejście do ekranu startowego</span><span class="sxs-lookup"><span data-stu-id="71ff5-107">Manually launch OneDrive by going to Start</span></span> ![Naciśnięcie klawisza Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="71ff5-109">, wpisz w polu wyszukiwania usługę OneDrive, a następnie kliknij aplikację klasyczną OneDrive.</span><span class="sxs-lookup"><span data-stu-id="71ff5-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="71ff5-110">**Resetowanie usługi OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="71ff5-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="71ff5-111">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="71ff5-111">Notes:</span></span>

- <span data-ttu-id="71ff5-112">Zresetowanie usługi OneDrive rozłącza wszystkie istniejące połączenia synchronizacji (w tym osobistą usługę OneDrive, jeśli jest skonfigurowana).</span><span class="sxs-lookup"><span data-stu-id="71ff5-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="71ff5-113">Nie utracisz plików ani danych, resetując usługę OneDrive na komputerze.</span><span class="sxs-lookup"><span data-stu-id="71ff5-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="71ff5-114">**Aby zresetować usługę OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="71ff5-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="71ff5-115">Otwórz okno dialogowe Uruchom, naciskając klawisze Windows i R.</span><span class="sxs-lookup"><span data-stu-id="71ff5-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="71ff5-116">Wpisz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i naciśnij przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="71ff5-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="71ff5-117">Okno polecenia może pojawić się krótko.</span><span class="sxs-lookup"><span data-stu-id="71ff5-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="71ff5-118">Ręczne uruchamianie usługi OneDrive przez przejście do ekranu startowego</span><span class="sxs-lookup"><span data-stu-id="71ff5-118">Manually launch OneDrive by going to Start</span></span> ![Naciśnięcie klawisza Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="71ff5-120">, wpisz w polu wyszukiwania usługę OneDrive, a następnie kliknij aplikację klasyczną OneDrive.</span><span class="sxs-lookup"><span data-stu-id="71ff5-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="71ff5-121">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="71ff5-121">Notes:</span></span>

- <span data-ttu-id="71ff5-122">Jeśli wybrano synchronizację tylko niektórych folderów przed zresetowaniem, musisz to zrobić ponownie po zakończeniu synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="71ff5-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="71ff5-123">Przeczytaj [artykuł Wybierz foldery usługi OneDrive do synchronizacji z komputerem, aby](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)uzyskać więcej   informacji.</span><span class="sxs-lookup"><span data-stu-id="71ff5-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="71ff5-124">Musisz to zrobić dla osobistej usługi OneDrive i usługi OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="71ff5-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>