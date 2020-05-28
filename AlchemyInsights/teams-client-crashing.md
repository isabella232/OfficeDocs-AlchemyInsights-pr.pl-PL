---
title: Awarie klienta usługi Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354062"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="63d19-102">Awarie klienta usługi Teams?</span><span class="sxs-lookup"><span data-stu-id="63d19-102">Teams client crashing?</span></span>

<span data-ttu-id="63d19-103">Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="63d19-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="63d19-104">Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="63d19-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="63d19-105">Upewnij się, że dostępne są wszystkie [adresy URL i zakresy adresów usługi Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="63d19-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="63d19-106">Zaloguj się przy użyciu konta administratora dzierżawy i sprawdź [pulpit nawigacyjny kondycji usługi,](https://docs.microsoft.com/office365/enterprise/view-service-health) aby sprawdzić, czy nie występuje awaria lub degradacja usługi.</span><span class="sxs-lookup"><span data-stu-id="63d19-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="63d19-107">Odinstalowywanie i ponowne instalowanie aplikacji Teams (łącze)</span><span class="sxs-lookup"><span data-stu-id="63d19-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="63d19-108">Przejdź do folderu %appdata%\Microsoft\teams\ na komputerze i usuń wszystkie pliki w tym katalogu.</span><span class="sxs-lookup"><span data-stu-id="63d19-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="63d19-109">[Pobierz i zainstaluj aplikację Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), a jeśli to możliwe, zainstaluj teams jako administratora (kliknij prawym przyciskiem myszy instalator teams i wybierz "Uruchom jako administrator", jeśli jest dostępny).</span><span class="sxs-lookup"><span data-stu-id="63d19-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="63d19-110">Jeśli twój klient usługi Teams nadal ulega awarii, czy możesz odtworzyć problem?</span><span class="sxs-lookup"><span data-stu-id="63d19-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="63d19-111">Jeśli tak:</span><span class="sxs-lookup"><span data-stu-id="63d19-111">If so:</span></span>

1. <span data-ttu-id="63d19-112">Użyj rejestratora kroków, aby uchwycić swoje kroki.</span><span class="sxs-lookup"><span data-stu-id="63d19-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="63d19-113">Zamknij WSZYSTKIE niepotrzebne lub poufne aplikacje.</span><span class="sxs-lookup"><span data-stu-id="63d19-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="63d19-114">Uruchom rejestrator kroków i odtwórz problem po zalogowaniu się za pomocą konta użytkownika, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="63d19-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="63d19-115">[Zbierz dzienniki zespołów, które przechwytują zarejestrowane kroki repro.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="63d19-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="63d19-116">**Uwaga:** Upewnij się, że przechwytujesz adres logowania użytkownika, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="63d19-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="63d19-117">Zbieranie informacji o zrzucie i/lub zasobniku błędów (Windows).</span><span class="sxs-lookup"><span data-stu-id="63d19-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="63d19-118">Uruchom program Windows Powershell na komputerze, na którym występuje awaria, i uruchom następujące polecenia:</span><span class="sxs-lookup"><span data-stu-id="63d19-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="63d19-119">Dołącz plik do sprawy pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="63d19-119">Attach the file to your support case.</span></span>
