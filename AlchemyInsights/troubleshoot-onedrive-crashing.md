---
title: Rozwiązywanie problemów z awariami usługi OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665008"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="e294c-102">Rozwiązywanie problemów z awariami usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="e294c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="e294c-103">Jeśli usługa OneDrive jest wielokrotnie awaria, spróbuj wykonać następujące czynności rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="e294c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="e294c-104">**Upewnij się, że klucze rejestru nie są ustawione:**</span><span class="sxs-lookup"><span data-stu-id="e294c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="e294c-105">Korzystanie z edytora rejestru przejdź do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="e294c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="e294c-106">Jeśli DisableFileSyncNGSC jest obecny i ustawiony na 1, Otwórz klucz i zmień wartość na 0.</span><span class="sxs-lookup"><span data-stu-id="e294c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="e294c-107">Ręcznie uruchom usługę OneDrive, przechodząc do ekranu startowego</span><span class="sxs-lookup"><span data-stu-id="e294c-107">Manually launch OneDrive by going to Start</span></span> ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e294c-109">Wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację klasyczną OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e294c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e294c-110">**Resetowanie usługi OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e294c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="e294c-111">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="e294c-111">Notes:</span></span>

- <span data-ttu-id="e294c-112">Zresetowanie usługi OneDrive powoduje odłączenie wszystkich istniejących połączeń synchronizacji (łącznie z osobistą usługą OneDrive, jeśli została skonfigurowana).</span><span class="sxs-lookup"><span data-stu-id="e294c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="e294c-113">Nie utracisz plików lub danych przez zresetowanie usługi OneDrive na komputerze.</span><span class="sxs-lookup"><span data-stu-id="e294c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="e294c-114">**Aby zresetować aplikację OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e294c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="e294c-115">Otwórz okno dialogowe Uruchamianie, naciskając klawisze Windows i R.</span><span class="sxs-lookup"><span data-stu-id="e294c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="e294c-116">Wpisz% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset i naciśnij przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="e294c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="e294c-117">Okno polecenia może być krótko wyświetlane.</span><span class="sxs-lookup"><span data-stu-id="e294c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="e294c-118">Ręcznie uruchom usługę OneDrive, przechodząc do ekranu startowego</span><span class="sxs-lookup"><span data-stu-id="e294c-118">Manually launch OneDrive by going to Start</span></span> ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e294c-120">Wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację klasyczną OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e294c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e294c-121">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="e294c-121">Notes:</span></span>

- <span data-ttu-id="e294c-122">Jeśli przed zresetowaniem wybrano opcję synchronizacji tylko niektóre foldery, konieczne będzie ponowne uruchomienie po zakończeniu synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="e294c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="e294c-123">Aby uzyskać więcej informacji, zobacz [Wybieranie folderów usługi OneDrive, które mają być synchronizowane z komputerem](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="e294c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="e294c-124">Musisz wykonać tę czynność dla swojej osobistej usługi OneDrive i usługi OneDrive dla firm.</span><span class="sxs-lookup"><span data-stu-id="e294c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>