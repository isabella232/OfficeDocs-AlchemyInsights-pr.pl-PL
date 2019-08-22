---
title: Dostęp do usług przejścia na emeryturę
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495761"
---
# <a name="access-services-retirement"></a><span data-ttu-id="65da4-102">Dostęp do usług przejścia na emeryturę</span><span class="sxs-lookup"><span data-stu-id="65da4-102">Access services retirement</span></span>

<span data-ttu-id="65da4-103">Jak pierwotnie ogłoszone w MC97576, w 2017 marca i nadal pozostawała w ubiegłym roku usług dostępu są wycofywane z usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="65da4-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="65da4-104">Kolejnym etapem w tym procesie będzie usunięcie sieci Web baz danych programu Access używać list programu SharePoint jako swojej podstawowej magazynu danych.</span><span class="sxs-lookup"><span data-stu-id="65da4-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="65da4-105">**Jak to wpływa na mnie?**</span><span class="sxs-lookup"><span data-stu-id="65da4-105">**How does this affect me?**</span></span>

<span data-ttu-id="65da4-106">Począwszy od czerwca 2019, będziemy zatrzymać tworzenie nowych baz danych programu Access w dokumentacji Online programu SharePoint i zamknij wszystkie pozostałe aplikacje i usługi 2020 kwietnia.</span><span class="sxs-lookup"><span data-stu-id="65da4-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="65da4-107">**Co trzeba zrobić, aby przygotować się na tę zmianę?**</span><span class="sxs-lookup"><span data-stu-id="65da4-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="65da4-108">Zachęcamy do tworzenia planu migracji dla baz danych web Access w organizacji.</span><span class="sxs-lookup"><span data-stu-id="65da4-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="65da4-109">Administratorzy można użyć [dostępu programu SharePoint aplikacji skanera](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) do uzyskania spis dostęp do aplikacji, które używają stron.</span><span class="sxs-lookup"><span data-stu-id="65da4-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="65da4-110">Istnieje kilka sposobów, aby przeprowadzić migrację danych baz danych programu Access w sieci web:</span><span class="sxs-lookup"><span data-stu-id="65da4-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="65da4-111">Importowanie z lokalną bazą danych programu Access (. ACCDB) lub do pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="65da4-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="65da4-112">Firma Microsoft zaleca, poznawanie Microsoft PowerApps jako alternatywna platforma do tworzenia rozwiązań biznesowych bez kodu dla sieci web i urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="65da4-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>