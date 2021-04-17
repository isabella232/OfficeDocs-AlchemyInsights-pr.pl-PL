---
title: Rozwiązywanie problemów z awariami usługi OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826209"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="75050-102">Rozwiązywanie problemów z awariami usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="75050-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="75050-103">Jeśli oneDrive wielokrotnie ulega awarii, spróbuj wykonać następujące kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="75050-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="75050-104">**Upewnij się, że klucze rejestru nie są ustawione:**</span><span class="sxs-lookup"><span data-stu-id="75050-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="75050-105">Za pomocą Edytora rejestru przejdź do HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="75050-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="75050-106">Jeśli wartość DisableFileSyncNGSC jest ustawiona na 1, otwórz klucz i zmień wartość na 0.</span><span class="sxs-lookup"><span data-stu-id="75050-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="75050-107">Ręczne uruchamianie aplikacji OneDrive przez uruchomienie</span><span class="sxs-lookup"><span data-stu-id="75050-107">Manually launch OneDrive by going to Start</span></span> ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="75050-109">, wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację komputerową OneDrive.</span><span class="sxs-lookup"><span data-stu-id="75050-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="75050-110">**Resetowanie aplikacji OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="75050-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="75050-111">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="75050-111">Notes:</span></span>

- <span data-ttu-id="75050-112">Zresetowanie aplikacji OneDrive powoduje odłączenie wszystkich istniejących połączeń synchronizacji (w tym twojej osobistej usługi OneDrive, jeśli je skonfiguruje).</span><span class="sxs-lookup"><span data-stu-id="75050-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="75050-113">Zresetowanie aplikacji OneDrive na komputerze nie spowoduje utraty plików ani danych.</span><span class="sxs-lookup"><span data-stu-id="75050-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="75050-114">**Aby zresetować usługę OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="75050-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="75050-115">Otwórz okno dialogowe Uruchamianie, naciskając klawisze Windows i R.</span><span class="sxs-lookup"><span data-stu-id="75050-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="75050-116">Wpisz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i naciśnij przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="75050-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="75050-117">Może zostać wyświetlone na krótko okno Polecenie.</span><span class="sxs-lookup"><span data-stu-id="75050-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="75050-118">Ręczne uruchamianie aplikacji OneDrive przez uruchomienie</span><span class="sxs-lookup"><span data-stu-id="75050-118">Manually launch OneDrive by going to Start</span></span> ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="75050-120">, wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację komputerową OneDrive.</span><span class="sxs-lookup"><span data-stu-id="75050-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="75050-121">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="75050-121">Notes:</span></span>

- <span data-ttu-id="75050-122">Jeśli przed zresetowaniu wybrano synchronizowanie tylko niektórych folderów, będzie konieczne ponowne ich zsynchronizowanie po ukończeniu synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="75050-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="75050-123">Przeczytaj [Wybieranie folderów usługi OneDrive do synchronizowania z komputerem, aby](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)uzyskać więcej   informacji.</span><span class="sxs-lookup"><span data-stu-id="75050-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="75050-124">Musisz to zrobić w przypadku osobistej usługi OneDrive i OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="75050-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>