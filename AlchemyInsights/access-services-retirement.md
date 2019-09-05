---
title: Dostęp do usług emerytalnych
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747794"
---
# <a name="access-services-retirement"></a><span data-ttu-id="f4b96-102">Dostęp do usług emerytalnych</span><span class="sxs-lookup"><span data-stu-id="f4b96-102">Access services retirement</span></span>

<span data-ttu-id="f4b96-103">Jak pierwotnie ogłosiliśmy w MC97576, w marcu 2017, i nadal komunikować się w ciągu ostatnich lat Access Services są wycofane z pakietu Office 365.</span><span class="sxs-lookup"><span data-stu-id="f4b96-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="f4b96-104">Następnym etapem w tym procesie będzie usunięcie baz danych programu Access w sieci Web, które używają list SharePoint jako ich podstawowej pamięci masowej.</span><span class="sxs-lookup"><span data-stu-id="f4b96-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="f4b96-105">**Jak to wpływa na mnie?**</span><span class="sxs-lookup"><span data-stu-id="f4b96-105">**How does this affect me?**</span></span>

<span data-ttu-id="f4b96-106">Począwszy od czerwca 2019, firma będzie zatrzymać tworzenie nowych baz danych programu Access w programie SharePoint Online i zamknąć usługę i wszystkie pozostałe aplikacje do kwietnia 2020.</span><span class="sxs-lookup"><span data-stu-id="f4b96-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="f4b96-107">**Co muszę zrobić, aby przygotować się do tej zmiany?**</span><span class="sxs-lookup"><span data-stu-id="f4b96-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="f4b96-108">Zachęcamy do utworzenia planu przejściowego dla baz danych programu Access w organizacji.</span><span class="sxs-lookup"><span data-stu-id="f4b96-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="f4b96-109">Administratorzy mogą używać [skanera aplikacji programu SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) do uzyskiwania spisu aplikacji programu Access korzystających z witryn.</span><span class="sxs-lookup"><span data-stu-id="f4b96-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="f4b96-110">Istnieje kilka sposobów migracji danych programu Access w sieci Web:</span><span class="sxs-lookup"><span data-stu-id="f4b96-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="f4b96-111">Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub do pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="f4b96-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="f4b96-112">Zalecamy również Eksplorowanie usługi Microsoft PowerApps jako alternatywnej platformy do tworzenia niekodowych rozwiązań biznesowych dla sieci Web i urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="f4b96-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>