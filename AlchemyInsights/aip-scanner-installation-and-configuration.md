---
title: 'Skaner AIP: instalacja i konfiguracja'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821673"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="229d2-102">Skaner AIP: instalacja i konfiguracja</span><span class="sxs-lookup"><span data-stu-id="229d2-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="229d2-103">**Aby zainstalować skaner AIP, postępuj zgodnie z zalecanymi wytycznymi:**</span><span class="sxs-lookup"><span data-stu-id="229d2-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="229d2-104">Jeśli uaktualniasz i nie wykonujesz czystej instalacji, upewnij się, że zostały przestrzegać wytycznych dotyczących uaktualniania skanera [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i ujednoliconego klienta etykiet, zobacz Uaktualnianie skanera Azure Information [Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="229d2-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="229d2-105">Upewnij się, że są spełnione wszystkie wymagania dotyczące [zapór i infrastruktury sieci.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="229d2-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="229d2-106">Upewnij się, [że zasady są ustawione na](https://docs.microsoft.com/azure/information-protection/configure-policy) etykiety automatyczne lub mają etykietę domyślną w zasadach.</span><span class="sxs-lookup"><span data-stu-id="229d2-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="229d2-107">Upewnij się, że odpowiedni typ pliku jest skonfigurowany do obsługi etykiet/ochrony zgodnie z opisem w tece Typy plików obsługiwane przez klienta [usługi Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="229d2-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="229d2-108">Ponadto, jeśli chcesz zmienić zachowanie domyślne, postępuj zgodnie z tymi wskazówkami: [Zmienianie domyślnego poziomu ochrony plików.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="229d2-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="229d2-109">Sprawdź, czy konto użytkownika skonfigurowane do uruchamiania usługi skanera ma uprawnienia dostępu do wszystkich skonfigurowanych repozytoriów.</span><span class="sxs-lookup"><span data-stu-id="229d2-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="229d2-110">Jeśli nadal masz problemy, wyeksportuj dzienniki skanera i dodaj je do biletu pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="229d2-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="229d2-111">**Eksportowanie dzienników skanera informacji o usłudze Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="229d2-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="229d2-112">W kontekście użytkownika z usługą skanera przejdź do lokalizacji %localappdata%\Microsoft\MSIP.</span><span class="sxs-lookup"><span data-stu-id="229d2-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="229d2-113">Spakuj całą zawartość w folderze MSIP.</span><span class="sxs-lookup"><span data-stu-id="229d2-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="229d2-114">Zapisz dzienniki w wybranej lokalizacji i dołącz je do zgłoszenia serwisowego.</span><span class="sxs-lookup"><span data-stu-id="229d2-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="229d2-115">Możesz również użyć funkcji [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="229d2-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="229d2-116">**Aby uzyskać dodatkowe informacje, zobacz:**</span><span class="sxs-lookup"><span data-stu-id="229d2-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="229d2-117">Wdrażanie programu Azure Information Protection w celu automatycznego klasyfikowania i chronienia plików</span><span class="sxs-lookup"><span data-stu-id="229d2-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="229d2-118">Określanie i używanie parametru Token w celu uwierzytelniania Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="229d2-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="229d2-119">Uruchamianie cyklu odnajdowania i wyświetlanie raportów dla skanera</span><span class="sxs-lookup"><span data-stu-id="229d2-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="229d2-120">Przejrzyj dokumentację usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="229d2-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="229d2-121">Wymagania dotyczące usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="229d2-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="229d2-122">Pobierz klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="229d2-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
