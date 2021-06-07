---
title: Nie można aktywować pakietu Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798690"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="6555d-102">Nie można aktywować pakietu Office</span><span class="sxs-lookup"><span data-stu-id="6555d-102">Unable to activate Office</span></span>

<span data-ttu-id="6555d-103">**Uwaga:** Jeśli korzystasz ze starszej wersji programu Windows (na przykład Windows 7), upewnij się, że domyślną obsługą jest TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="6555d-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="6555d-104">Aby uzyskać więcej informacji, zobacz Aktualizowanie w celu włączenia [protokołów TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako domyślnych protokołów bezpiecznego w winieHTTP w Windows.</span><span class="sxs-lookup"><span data-stu-id="6555d-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="6555d-105">Sprawdź, czy stan Twojej subskrypcji wskazuje, że upłynęła jej ważność.</span><span class="sxs-lookup"><span data-stu-id="6555d-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="6555d-106">Upewnij się, że masz subskrypcję zezwalającą na licencje klienta, np. Office 365 Business lub Business Premium, oraz [upewnij się, że użytkownik ma przypisaną licencję](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="6555d-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="6555d-107">Upewnij się, że użytkownik loguje się do pakietu Office za pomocą tego samego konta, do którego jest przypisana licencja.</span><span class="sxs-lookup"><span data-stu-id="6555d-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="6555d-108">Sprawdź [stronę kondycji usługi Office 365](/office365/enterprise/view-service-health), aby zobaczyć, czy opisano na niej znane problemy z tą usługą.</span><span class="sxs-lookup"><span data-stu-id="6555d-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="6555d-109">Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu aplikacji platformy Microsoft 365 do Internetu.</span><span class="sxs-lookup"><span data-stu-id="6555d-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="6555d-110">Zobacz [Adresy URL i zakresy adresów IP usługi Office 365](/office365/enterprise/urls-and-ip-address-ranges "Adresy URL i zakresy adresów IP usługi Office 365").</span><span class="sxs-lookup"><span data-stu-id="6555d-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="6555d-111">**Porada** Na komputerach z systemem Windows możemy diagnozować i automatycznie rozwiązywać wiele typowych problemów z logowaniem do pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="6555d-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="6555d-112">Pobierz i uruchom  **[Asystenta odzyskiwania i pomocy technicznej dla usługi Office 365](https://aka.ms/SaRA-OfficeSignInScenario)**, aby skorzystać z naszego zautomatyzowanego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="6555d-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="6555d-113">Wykonaj następujące czynności rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="6555d-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="6555d-114">Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6555d-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="6555d-115">[Usuń](/microsoft-365/admin/manage/remove-licenses-from-users) i [przypisz ponownie](/microsoft-365/admin/manage/assign-licenses-to-users) licencję pakietu Office, a następnie [zaloguj się do pakietu Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="6555d-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="6555d-116">Uruchamianie [narzędzia do rozwiązywania problemów z aktywacją](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="6555d-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="6555d-117">Resetowanie stanu aktywacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="6555d-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Resetowanie stanu aktywacji pakietu Office")
- [<span data-ttu-id="6555d-118">Wykonywanie naprawy online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="6555d-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="6555d-119">Aby poznać dodatkowe rozwiązania do rozwiązywania problemów, zobacz:</span><span class="sxs-lookup"><span data-stu-id="6555d-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="6555d-120">Błędy „Produkt bez licencji” i błędy aktywacji w pakiecie Office</span><span class="sxs-lookup"><span data-stu-id="6555d-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="6555d-121">Błąd „Niestety, nie można nawiązać połączenia z kontem. Spróbuj ponownie później” podczas aktywowania pakietu Office</span><span class="sxs-lookup"><span data-stu-id="6555d-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)