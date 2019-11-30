---
title: Problem z aktywacją-nie możemy się połączyć już teraz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628252"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="ea779-102">Naprawianie aplikacji pakietu Office "nie jesteśmy w stanie połączyć się teraz" wiadomość</span><span class="sxs-lookup"><span data-stu-id="ea779-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="ea779-103">Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ea779-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ea779-104">Sprawdź ustawienia zapory sieciowej, oprogramowania antywirusowego i serwera proxy, aby potwierdzić, że nie blokują dostępu do Internetu aplikacjom pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ea779-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ea779-105">Zobacz [adresy url 365 pakietu Office i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ea779-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ea779-106">Przejdź do **Start** > **Run**, a następnie wpisz **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="ea779-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ea779-107">Upewnij się, że są uruchomione następujące usługi:</span><span class="sxs-lookup"><span data-stu-id="ea779-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ea779-108">Automatyczna konfiguracja urządzeń podłączonych do sieci</span><span class="sxs-lookup"><span data-stu-id="ea779-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ea779-109">Usługa listy sieci</span><span class="sxs-lookup"><span data-stu-id="ea779-109">Network List Service</span></span>
    - <span data-ttu-id="ea779-110">Rozpoznawanie lokalizacji w sieci</span><span class="sxs-lookup"><span data-stu-id="ea779-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ea779-111">Dziennik zdarzeń systemu Windows</span><span class="sxs-lookup"><span data-stu-id="ea779-111">Windows Event Log</span></span>

<span data-ttu-id="ea779-112">Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić.</span><span class="sxs-lookup"><span data-stu-id="ea779-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ea779-113">Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="ea779-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ea779-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="ea779-114">**sfc /scannow**</span></span>

<span data-ttu-id="ea779-115">Po zakończeniu tego polecenia Uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="ea779-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ea779-116">Aby uzyskać szczegółowe informacje, zobacz ["Przepraszamy, nie możemy nawiązać połączenia z Twoim kontem. Spróbuj ponownie później "błąd podczas aktywowania pakietu Office z pakietu Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ea779-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>