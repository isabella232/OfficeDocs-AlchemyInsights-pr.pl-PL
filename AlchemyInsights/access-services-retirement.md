---
title: Przejście na emeryturę usług dostępu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687268"
---
# <a name="access-services-retirement"></a><span data-ttu-id="c1e1d-102">Przejście na emeryturę usług dostępu</span><span class="sxs-lookup"><span data-stu-id="c1e1d-102">Access services retirement</span></span>

<span data-ttu-id="c1e1d-103">Jak pierwotnie ogłosiliśmy w MC97576, w marcu 2017 r., i nadal komunikować się w ciągu ostatniego roku Usługi dostępu są na emeryturze.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="c1e1d-104">Następną fazą tego procesu będzie usunięcie baz danych sieci Web programu Access, które używają list programu SharePoint jako bazowego magazynu danych.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="c1e1d-105">**Jak to wpływa na mnie?**</span><span class="sxs-lookup"><span data-stu-id="c1e1d-105">**How does this affect me?**</span></span>

<span data-ttu-id="c1e1d-106">Od czerwca 2019 r. przestaniemy tworzenie nowych baz danych programu Access w usłudze SharePoint Online i do kwietnia 2020 r. wyłączymy usługę i wszystkie pozostałe aplikacje.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="c1e1d-107">**Co muszę zrobić, aby przygotować się do tej zmiany?**</span><span class="sxs-lookup"><span data-stu-id="c1e1d-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="c1e1d-108">Zachęcamy do utworzenia planu przejścia dla baz danych sieci Web programu Access w organizacji.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="c1e1d-109">Administratorzy mogą korzystać ze [skanera aplikacji programu SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) w celu uzyskania spisu aplikacji programu Access używanych przez witryny.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="c1e1d-110">Istnieje kilka sposobów migracji danych baz danych sieci Web programu Access:</span><span class="sxs-lookup"><span data-stu-id="c1e1d-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="c1e1d-111">Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub do pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="c1e1d-112">Zalecamy również zbadanie usługi Microsoft PowerApps jako alternatywnej platformy do tworzenia rozwiązań biznesowych bez kodu dla urządzeń sieci Web i urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="c1e1d-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>