---
title: Awarie klienta usługi Teams?
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826281"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="910ac-102">Awarie klienta usługi Teams?</span><span class="sxs-lookup"><span data-stu-id="910ac-102">Teams client crashing?</span></span>

<span data-ttu-id="910ac-103">Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="910ac-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="910ac-104">Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="910ac-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="910ac-105">Upewnij się, że wszystkie adresy URL i zakresy adresów platformy [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) są dostępne.</span><span class="sxs-lookup"><span data-stu-id="910ac-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="910ac-106">Zaloguj się przy użyciu konta administratora dzierżawy i sprawdź pulpit [nawigacyjny](https://docs.microsoft.com/office365/enterprise/view-service-health) kondycji usługi, aby sprawdzić, czy nie występuje żadne uszkodzenie lub obniżenie wydajności usługi.</span><span class="sxs-lookup"><span data-stu-id="910ac-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="910ac-107">Odinstalowanie i ponowne zainstalowanie aplikacji Teams (link)</span><span class="sxs-lookup"><span data-stu-id="910ac-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="910ac-108">Przejdź do folderu %appdata%\Microsoft\teams\ na komputerze i usuń wszystkie pliki w tym katalogu.</span><span class="sxs-lookup"><span data-stu-id="910ac-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="910ac-109">[Pobierz i zainstaluj aplikację Teams,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a jeśli to możliwe, zainstaluj aplikację Teams jako administrator (kliknij prawym przyciskiem myszy instalator Teams i wybierz opcję "Uruchom jako administrator", jeśli jest dostępny).</span><span class="sxs-lookup"><span data-stu-id="910ac-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="910ac-110">Jeśli klient usługi Teams nadal ulega awarii, czy możesz odtworzyć problem?</span><span class="sxs-lookup"><span data-stu-id="910ac-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="910ac-111">Jeśli tak jest:</span><span class="sxs-lookup"><span data-stu-id="910ac-111">If so:</span></span>

1. <span data-ttu-id="910ac-112">Skorzystaj z Rejestratora problemów, aby przechwycić czynności.</span><span class="sxs-lookup"><span data-stu-id="910ac-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="910ac-113">Zamknij WSZYSTKIE zbędne lub poufne aplikacje.</span><span class="sxs-lookup"><span data-stu-id="910ac-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="910ac-114">Uruchom Rejestratora problemów i odtprodukuj problem po zalogowaniu się przy użyciu odpowiedniego konta użytkownika.</span><span class="sxs-lookup"><span data-stu-id="910ac-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="910ac-115">[Zbierz dzienniki zespołów, które przechwytują zarejestrowane kroki ponownego przekierowy.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="910ac-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="910ac-116">**Uwaga:** upewnij się, że przechwycono adres logowania użytkownika, u który ma wpływ.</span><span class="sxs-lookup"><span data-stu-id="910ac-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="910ac-117">Zbierz zrzut i/lub informacje zasobnika błędów (Windows).</span><span class="sxs-lookup"><span data-stu-id="910ac-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="910ac-118">Uruchom program Windows PowerShell na komputerze, na którym występuje awaria, i uruchom następujące polecenia:</span><span class="sxs-lookup"><span data-stu-id="910ac-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="910ac-119">Dołącz plik do sprawy pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="910ac-119">Attach the file to your support case.</span></span>
