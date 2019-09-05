---
title: Zapisywanie witryny lub listy jako szablonu
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752042"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="0775d-102">Zapisywanie witryny lub listy jako szablonu</span><span class="sxs-lookup"><span data-stu-id="0775d-102">Save site or list as a template</span></span>

<span data-ttu-id="0775d-103">Szablony witryn programu SharePoint są wstępnie skompilowanymi definicjami zaprojektowanymi wokół konkretnej potrzeby biznesowej.</span><span class="sxs-lookup"><span data-stu-id="0775d-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="0775d-104">Aby uzyskać więcej informacji, zobacz [za pomocą szablonów do tworzenia różnych rodzajów witryn programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="0775d-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="0775d-105">Oto kilka typowych problemów/rozwiązań dotyczących zapisywania witryny lub listy jako szablon w programie SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="0775d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="0775d-106">**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brak**.</span><span class="sxs-lookup"><span data-stu-id="0775d-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="0775d-107">Administratorzy będą musieli zezwolić na skrypt niestandardowy, aby włączyć funkcje szablonu.</span><span class="sxs-lookup"><span data-stu-id="0775d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="0775d-108">Szczegółowe kroki, przykłady i zagadnienia zobacz [Zezwalaj lub zapobieganie skryptu niestandardowego](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="0775d-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="0775d-109">Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy w witrynach, które korzystają z infrastruktury publikowania programu SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="0775d-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="0775d-110">**Nie można utworzyć szablonu witryny lub nie działa poprawnie**</span><span class="sxs-lookup"><span data-stu-id="0775d-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="0775d-111">Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie uaktywni się.</span><span class="sxs-lookup"><span data-stu-id="0775d-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="0775d-112">Jeśli funkcja nie jest dostępna do aktywowania w bieżącym zbiorze witryn, nie można użyć szablonu witryny do utworzenia witryny.</span><span class="sxs-lookup"><span data-stu-id="0775d-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="0775d-113">Sprawdź, czy wszystkie listy lub biblioteki przekraczają [próg limitu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 elementów, ponieważ może to blokować Tworzenie szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="0775d-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="0775d-114">Witryna może używać zbyt wielu zasobów i dlatego szablon witryny przekracza limit 50 megabajtów (MB).</span><span class="sxs-lookup"><span data-stu-id="0775d-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="0775d-115">Istnieją problemy z wyświetlaniem danych z listy, która używa kolumny odnośnika.</span><span class="sxs-lookup"><span data-stu-id="0775d-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="0775d-116">Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablon nie wyświetla danych z listy wyszukiwania poprawne w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="0775d-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="0775d-117">Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, należy odwoływać się, [tworzyć i używać szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="0775d-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

