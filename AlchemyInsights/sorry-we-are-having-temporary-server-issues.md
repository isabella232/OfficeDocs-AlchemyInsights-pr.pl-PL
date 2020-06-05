---
title: Naprawianie aplikacji Microsoft 365 Niestety, mamy tymczasowy komunikat o problemach z serwerem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582713"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="56ed1-102">Naprawianie komunikatu "Przepraszamy, mamy tymczasowe problemy z serwerem"</span><span class="sxs-lookup"><span data-stu-id="56ed1-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="56ed1-103">Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="56ed1-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="56ed1-104">Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują dostępu do Internetu do aplikacji usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="56ed1-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="56ed1-105">Zobacz [adresy URL i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="56ed1-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="56ed1-106">Przejdź do **ekranu**  >  **Uruchom**, a następnie wpisz **plik services.msc**.</span><span class="sxs-lookup"><span data-stu-id="56ed1-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="56ed1-107">Upewnij się, że wszystkie następujące usługi są uruchomione:</span><span class="sxs-lookup"><span data-stu-id="56ed1-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="56ed1-108">Automatyczna konfiguracja urządzeń podłączonych do sieci</span><span class="sxs-lookup"><span data-stu-id="56ed1-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="56ed1-109">Usługa listy sieci</span><span class="sxs-lookup"><span data-stu-id="56ed1-109">Network List Service</span></span>
    - <span data-ttu-id="56ed1-110">Rozpoznawanie lokalizacji sieciowej</span><span class="sxs-lookup"><span data-stu-id="56ed1-110">Network Location Awareness</span></span>
    - <span data-ttu-id="56ed1-111">Dziennik zdarzeń systemu Windows</span><span class="sxs-lookup"><span data-stu-id="56ed1-111">Windows Event Log</span></span>

<span data-ttu-id="56ed1-112">Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić.</span><span class="sxs-lookup"><span data-stu-id="56ed1-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="56ed1-113">Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="56ed1-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="56ed1-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="56ed1-114">**sfc /scannow**</span></span>

<span data-ttu-id="56ed1-115">Po zakończeniu tego polecenia uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="56ed1-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="56ed1-116">Aby uzyskać szczegółowe informacje, zobacz ["Przepraszamy, nie możemy połączyć się z Twoim kontem. Spróbuj ponownie później" błąd po aktywacji](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="56ed1-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>