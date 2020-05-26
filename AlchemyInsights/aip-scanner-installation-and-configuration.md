---
title: 'Skaner AIP: instalacja i konfiguracja'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358103"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="5ab14-102">Skaner AIP: instalacja i konfiguracja</span><span class="sxs-lookup"><span data-stu-id="5ab14-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="5ab14-103">**Aby zainstalować skaner AIP, postępuj zgodnie z zalecanymi wytycznymi:**</span><span class="sxs-lookup"><span data-stu-id="5ab14-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="5ab14-104">Jeśli uaktualniasz i nie wykonujesz czystej instalacji, upewnij się, że przestrzegałeś wskazówek dotyczących [uaktualniania skanera usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i ujednoliconego klienta etykietowania, zobacz [uaktualnianie skanera usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="5ab14-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="5ab14-105">Sprawdź, czy są zgodne ze [wszystkimi zapory i wymagania dotyczące ustawień infrastruktury sieciowej](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="5ab14-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="5ab14-106">Upewnij się, że [zasady są ustawione](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatyczne etykietowanie lub mają domyślną etykietę w zasadach.</span><span class="sxs-lookup"><span data-stu-id="5ab14-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="5ab14-107">Upewnij się, że odpowiedni typ pliku jest skonfigurowany pod kątem etykiety/ochrony zgodnie z opisem w [obszarze Typy plików obsługiwane przez klienta usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="5ab14-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="5ab14-108">Ponadto, jeśli chcesz zmienić zachowanie domyślne, postępuj zgodnie z tymi wskazówkami: [Zmiana domyślnego poziomu ochrony plików](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="5ab14-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="5ab14-109">Sprawdź, czy konto użytkownika skonfigurowane do uruchamiania usługi skanera ma uprawnienia dostępu do wszystkich skonfigurowanych repozytoriów.</span><span class="sxs-lookup"><span data-stu-id="5ab14-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="5ab14-110">Jeśli nadal występują problemy, wyeksportuj dzienniki skanera i dodaj je do biletu pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="5ab14-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="5ab14-111">**Eksportowanie dzienników skanera ochrony informacji platformy Azure**</span><span class="sxs-lookup"><span data-stu-id="5ab14-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="5ab14-112">Przejdź do %localappdata%\Microsoft\MSIP w kontekście użytkownika z uruchomieniem usługi skanera.</span><span class="sxs-lookup"><span data-stu-id="5ab14-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="5ab14-113">Siąz całą zawartość w folderze MSIP.</span><span class="sxs-lookup"><span data-stu-id="5ab14-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="5ab14-114">Zapisz dzienniki w wybranej lokalizacji i dołącz je do żądania usługi.</span><span class="sxs-lookup"><span data-stu-id="5ab14-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="5ab14-115">Można również użyć [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="5ab14-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="5ab14-116">**Aby uzyskać dodatkowe informacje, zobacz:**</span><span class="sxs-lookup"><span data-stu-id="5ab14-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="5ab14-117">Wdrażanie skanera usługi Azure Information Protection w celu automatycznego klasyfikowania i ochrony plików</span><span class="sxs-lookup"><span data-stu-id="5ab14-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="5ab14-118">Określanie i używanie parametru Token dla set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="5ab14-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="5ab14-119">Uruchamianie cyklu odnajdowania i wyświetlanie raportów dla skanera</span><span class="sxs-lookup"><span data-stu-id="5ab14-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="5ab14-120">Zapoznaj się z dokumentacją usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5ab14-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="5ab14-121">Wymagania dotyczące usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5ab14-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="5ab14-122">Pobierz klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5ab14-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
