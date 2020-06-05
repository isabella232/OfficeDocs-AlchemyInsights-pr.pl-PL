---
title: Problem z aktywacją - Nie możemy teraz połączyć się
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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581885"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="d09fc-102">Naprawianie komunikatu "Nie możemy teraz połączyć się z aplikacjami usługi Microsoft 365"</span><span class="sxs-lookup"><span data-stu-id="d09fc-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="d09fc-103">Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="d09fc-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d09fc-104">Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują dostępu do Internetu do aplikacji usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d09fc-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d09fc-105">Zobacz [adresy URL firmy Microsoft i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d09fc-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d09fc-106">Przejdź do **ekranu**  >  **Uruchom**, a następnie wpisz **plik services.msc**.</span><span class="sxs-lookup"><span data-stu-id="d09fc-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d09fc-107">Upewnij się, że wszystkie następujące usługi są uruchomione:</span><span class="sxs-lookup"><span data-stu-id="d09fc-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d09fc-108">Automatyczna konfiguracja urządzeń podłączonych do sieci</span><span class="sxs-lookup"><span data-stu-id="d09fc-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d09fc-109">Usługa listy sieci</span><span class="sxs-lookup"><span data-stu-id="d09fc-109">Network List Service</span></span>
    - <span data-ttu-id="d09fc-110">Rozpoznawanie lokalizacji sieciowej</span><span class="sxs-lookup"><span data-stu-id="d09fc-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d09fc-111">Dziennik zdarzeń systemu Windows</span><span class="sxs-lookup"><span data-stu-id="d09fc-111">Windows Event Log</span></span>

<span data-ttu-id="d09fc-112">Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić.</span><span class="sxs-lookup"><span data-stu-id="d09fc-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d09fc-113">Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="d09fc-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d09fc-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="d09fc-114">**sfc /scannow**</span></span>

<span data-ttu-id="d09fc-115">Po zakończeniu tego polecenia uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="d09fc-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d09fc-116">Aby uzyskać szczegółowe informacje, zobacz ["Przepraszamy, nie możemy połączyć się z Twoim kontem. Spróbuj ponownie później" błąd po przyśpiesze office z usługi Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="d09fc-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>