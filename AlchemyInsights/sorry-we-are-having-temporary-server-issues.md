---
title: Rozwiązywanie problemów z aplikacjami Microsoft 365 Przepraszamy, mamy komunikat o tymczasowych problemach z serwerem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758255"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="a21f4-102">Rozwiązywanie problemów z aplikacjami Microsoft 365 "Niestety, występują tymczasowe problemy z serwerami"</span><span class="sxs-lookup"><span data-stu-id="a21f4-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="a21f4-103">Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a21f4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a21f4-104">Sprawdź ustawienia zapory, oprogramowania antywirusowego i ustawień serwera proxy, aby upewnić się, że nie blokuje dostępu do Internetu aplikacjom Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a21f4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a21f4-105">Zobacz [adresy URL i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a21f4-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a21f4-106">Przejdź do **ekranu startowego**  >  **Run**, a następnie wpisz **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="a21f4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a21f4-107">Upewnij się, że są uruchomione następujące usługi:</span><span class="sxs-lookup"><span data-stu-id="a21f4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a21f4-108">Automatyczne konfigurowanie urządzeń podłączonych do sieci</span><span class="sxs-lookup"><span data-stu-id="a21f4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a21f4-109">Usługa listy sieci</span><span class="sxs-lookup"><span data-stu-id="a21f4-109">Network List Service</span></span>
    - <span data-ttu-id="a21f4-110">Rozpoznawanie lokalizacji w sieci</span><span class="sxs-lookup"><span data-stu-id="a21f4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a21f4-111">Dziennik zdarzeń systemu Windows</span><span class="sxs-lookup"><span data-stu-id="a21f4-111">Windows Event Log</span></span>

<span data-ttu-id="a21f4-112">Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić.</span><span class="sxs-lookup"><span data-stu-id="a21f4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a21f4-113">Jeśli wystąpił problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="a21f4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a21f4-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="a21f4-114">**sfc /scannow**</span></span>

<span data-ttu-id="a21f4-115">Po zakończeniu tego polecenia Uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="a21f4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a21f4-116">Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można nawiązać połączenia z kontem. Podczas aktywowania spróbuj ponownie później](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a21f4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>