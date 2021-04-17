---
title: Rozwiązywanie problemów z aplikacjami platformy Microsoft 365 Niestety, mamy komunikat o tymczasowych problemach z serwerem
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835281"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="0db94-102">Naprawianie aplikacji platformy Microsoft 365 Komunikat "Niestety, mamy problemy z serwerem tymczasowych"</span><span class="sxs-lookup"><span data-stu-id="0db94-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="0db94-103">Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="0db94-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0db94-104">Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu do aplikacji platformy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0db94-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="0db94-105">Zobacz [Adresy URL i zakresy adresów IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="0db94-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0db94-106">Przejdź do  >  **startowego uruchamiania**, a następnie wpisz **services.msc.**</span><span class="sxs-lookup"><span data-stu-id="0db94-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0db94-107">Upewnij się, że wszystkie następujące usługi są uruchomione:</span><span class="sxs-lookup"><span data-stu-id="0db94-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0db94-108">Automatyczne konfigurowanie urządzeń połączonych z siecią</span><span class="sxs-lookup"><span data-stu-id="0db94-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0db94-109">Usługa listy sieciowej</span><span class="sxs-lookup"><span data-stu-id="0db94-109">Network List Service</span></span>
    - <span data-ttu-id="0db94-110">Informacje o lokalizacji sieciowej</span><span class="sxs-lookup"><span data-stu-id="0db94-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0db94-111">Dziennik zdarzeń systemu Windows</span><span class="sxs-lookup"><span data-stu-id="0db94-111">Windows Event Log</span></span>

<span data-ttu-id="0db94-112">Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić.</span><span class="sxs-lookup"><span data-stu-id="0db94-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0db94-113">Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="0db94-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0db94-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="0db94-114">**sfc /scannow**</span></span>

<span data-ttu-id="0db94-115">Po zakończeniu tego polecenia uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="0db94-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0db94-116">Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można połączyć się z Twoim kontem. Spróbuj ponownie później" podczas aktywowania](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="0db94-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>