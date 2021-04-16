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
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812582"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="3a02c-102">Nie można aktywować pakietu Office</span><span class="sxs-lookup"><span data-stu-id="3a02c-102">Unable to activate Office</span></span>

- <span data-ttu-id="3a02c-103">Sprawdź, czy stan Twojej subskrypcji wskazuje, że upłynęła jej ważność.</span><span class="sxs-lookup"><span data-stu-id="3a02c-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="3a02c-104">Upewnij się, że masz subskrypcję zezwalającą na licencje klienta, np. Office 365 Business lub Business Premium, oraz [upewnij się, że użytkownik ma przypisaną licencję](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3a02c-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="3a02c-105">Upewnij się, że użytkownik loguje się do pakietu Office za pomocą tego samego konta, do którego jest przypisana licencja.</span><span class="sxs-lookup"><span data-stu-id="3a02c-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="3a02c-106">Sprawdź [stronę kondycji usługi Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health), aby zobaczyć, czy opisano na niej znane problemy z tą usługą.</span><span class="sxs-lookup"><span data-stu-id="3a02c-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="3a02c-107">Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu aplikacji platformy Microsoft 365 do Internetu.</span><span class="sxs-lookup"><span data-stu-id="3a02c-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="3a02c-108">Zobacz [Adresy URL i zakresy adresów IP usługi Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Adresy URL i zakresy adresów IP usługi Office 365").</span><span class="sxs-lookup"><span data-stu-id="3a02c-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="3a02c-109">**Porada** Na komputerach z systemem Windows możemy diagnozować i automatycznie rozwiązywać wiele typowych problemów z logowaniem do pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="3a02c-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="3a02c-110">Pobierz i uruchom  **[Asystenta odzyskiwania i pomocy technicznej dla usługi Office 365](https://aka.ms/SaRA-OfficeSignInScenario)**, aby skorzystać z naszego zautomatyzowanego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="3a02c-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="3a02c-111">Wykonaj następujące czynności rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="3a02c-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="3a02c-112">Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3a02c-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="3a02c-113">[Usuń](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [przypisz ponownie](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencję pakietu Office, a następnie [zaloguj się do pakietu Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="3a02c-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="3a02c-114">Uruchamianie [narzędzia do rozwiązywania problemów z aktywacją](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="3a02c-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="3a02c-115">Resetowanie stanu aktywacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="3a02c-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Resetowanie stanu aktywacji pakietu Office")
- [<span data-ttu-id="3a02c-116">Wykonywanie naprawy online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="3a02c-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="3a02c-117">Aby poznać dodatkowe rozwiązania do rozwiązywania problemów, zobacz:</span><span class="sxs-lookup"><span data-stu-id="3a02c-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="3a02c-118">Błędy „Produkt bez licencji” i błędy aktywacji w pakiecie Office</span><span class="sxs-lookup"><span data-stu-id="3a02c-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="3a02c-119">Błąd „Niestety, nie można nawiązać połączenia z kontem. Spróbuj ponownie później” podczas aktywowania pakietu Office</span><span class="sxs-lookup"><span data-stu-id="3a02c-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)