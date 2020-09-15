---
title: Wycofanie usług programu Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698692"
---
# <a name="access-services-retirement"></a><span data-ttu-id="80e7d-102">Wycofanie usług programu Access</span><span class="sxs-lookup"><span data-stu-id="80e7d-102">Access services retirement</span></span>

<span data-ttu-id="80e7d-103">Ponieważ został pierwotnie ogłoszony w MC97576, w marcu 2017 r. i kontynuując komunikację w ciągu ubiegłych rocznych usług programu Access.</span><span class="sxs-lookup"><span data-stu-id="80e7d-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="80e7d-104">Kolejnym etapem tego procesu będzie usunięcie baz danych sieci Web programu Access, które używają list programu SharePoint jako podstawowego magazynu danych.</span><span class="sxs-lookup"><span data-stu-id="80e7d-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="80e7d-105">**Jak to wpłynie?**</span><span class="sxs-lookup"><span data-stu-id="80e7d-105">**How does this affect me?**</span></span>

<span data-ttu-id="80e7d-106">Począwszy od czerwca 2019, my zakończymy tworzenie nowych baz danych programu Access w usłudze SharePoint Online oraz zamkniją usługę i wszystkie pozostałe aplikacje do 2020 kwietnia.</span><span class="sxs-lookup"><span data-stu-id="80e7d-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="80e7d-107">**Co muszę zrobić, aby przygotować się na tę zmianę?**</span><span class="sxs-lookup"><span data-stu-id="80e7d-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="80e7d-108">Zachęcamy do utworzenia planu migracji dla baz danych sieci Web programu Access w organizacji.</span><span class="sxs-lookup"><span data-stu-id="80e7d-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="80e7d-109">Administratorzy mogą korzystać ze [skanera aplikacji programu SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) w celu uzyskania spisu aplikacji programu Access, których używają witryny.</span><span class="sxs-lookup"><span data-stu-id="80e7d-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="80e7d-110">Istnieje kilka sposobów migrowania danych baz danych sieci Web programu Access:</span><span class="sxs-lookup"><span data-stu-id="80e7d-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="80e7d-111">Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="80e7d-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="80e7d-112">Zalecamy również Eksplorowanie usługi Microsoft PowerApps jako alternatywnej platformy, która umożliwia tworzenie bez kodu rozwiązania biznesowego dla sieci Web i urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="80e7d-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>