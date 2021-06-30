---
title: Teams awarie klienta
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
- "9002323"
- "4512"
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187731"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="6b325-102">Teams awarie klienta</span><span class="sxs-lookup"><span data-stu-id="6b325-102">Teams client crashing</span></span>

<span data-ttu-id="6b325-103">Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="6b325-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="6b325-104">Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="6b325-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="6b325-105">Upewnij się, że [wszystkie Microsoft 365 URL i zakresy adresów](/microsoftteams/connectivity-issues) są dostępne.</span><span class="sxs-lookup"><span data-stu-id="6b325-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="6b325-106">Zaloguj się przy użyciu konta administratora dzierżawy i sprawdź pulpit [nawigacyjny](/office365/enterprise/view-service-health) kondycji usługi, aby sprawdzić, czy nie występuje żadne uszkodzenie lub obniżenie wydajności usługi.</span><span class="sxs-lookup"><span data-stu-id="6b325-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="6b325-107">Odinstaluj i ponownie zainstaluj aplikację Teams.</span><span class="sxs-lookup"><span data-stu-id="6b325-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="6b325-108">Przejdź do folderu %appdata%\Microsoft\Teams\ na komputerze i usuń wszystkie pliki w tym katalogu.</span><span class="sxs-lookup"><span data-stu-id="6b325-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="6b325-109">[Pobierz i zainstaluj aplikację pakietu Teams,](https://www.microsoft.com/microsoft-teams/download-app)a jeśli to możliwe, zainstaluj aplikację Teams jako administrator (kliknij prawym przyciskiem myszy instalatora Teams i wybierz polecenie Uruchom jako **administrator, jeśli** jest dostępne).</span><span class="sxs-lookup"><span data-stu-id="6b325-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="6b325-110">Jeśli Teams nadal ulega awarii, spróbuj odtworzyć problem.</span><span class="sxs-lookup"><span data-stu-id="6b325-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="6b325-111">Jeśli możesz:</span><span class="sxs-lookup"><span data-stu-id="6b325-111">If you can:</span></span>

1. <span data-ttu-id="6b325-112">Skorzystaj z Rejestratora problemów, aby przechwycić czynności.</span><span class="sxs-lookup"><span data-stu-id="6b325-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="6b325-113">Zamknij WSZYSTKIE zbędne lub poufne aplikacje.</span><span class="sxs-lookup"><span data-stu-id="6b325-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="6b325-114">Uruchom Rejestratora problemów i odtprodukuj problem po zalogowaniu się przy użyciu odpowiedniego konta użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6b325-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="6b325-115">[Zbierz dzienniki zespołów, które przechwytują zarejestrowane kroki ponownego przekierowy.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="6b325-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="6b325-116">**Uwaga:** upewnij się, że przechwycono adres logowania użytkownika, u który ma wpływ.</span><span class="sxs-lookup"><span data-stu-id="6b325-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="6b325-117">Zbierz zrzut i/lub informacje zasobnika błędów (Windows).</span><span class="sxs-lookup"><span data-stu-id="6b325-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="6b325-118">Uruchom Windows PowerShell na komputerze, na którym występuje awaria, i uruchom następujące polecenia (po każdym z poleceń naciśnij klawisz Enter):</span><span class="sxs-lookup"><span data-stu-id="6b325-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="6b325-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="6b325-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="6b325-120">Po wygenerowaniu pliku tekstowego, który pojawi się na ekranie, zapisz go i dołącz do żądania usługi.</span><span class="sxs-lookup"><span data-stu-id="6b325-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
