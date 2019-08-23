---
title: Zapisz jako szablon witryny lub listy
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551641"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="b265f-102">Zapisz jako szablon witryny lub listy</span><span class="sxs-lookup"><span data-stu-id="b265f-102">Save site or list as a template</span></span>

<span data-ttu-id="b265f-103">Szablony witryn programu SharePoint są wbudowane definicje została zaprojektowana dla określonych potrzeb biznesowych.</span><span class="sxs-lookup"><span data-stu-id="b265f-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="b265f-104">Aby uzyskać więcej informacji zobacz [Używanie szablonów do tworzenia różnego rodzaju witryny programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="b265f-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="b265f-105">Poniżej przedstawiono typowe problemy/rozwiązania dotyczące zapisywania witryny lub listy jako szablonu w dokumentacji Online programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b265f-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="b265f-106">**Zapisz witrynę/lista przycisk Szablon nie jest dostępne lub brak**.</span><span class="sxs-lookup"><span data-stu-id="b265f-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="b265f-107">Administratorzy należy umożliwić niestandardowego skryptu do włączenia funkcji szablonu.</span><span class="sxs-lookup"><span data-stu-id="b265f-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="b265f-108">Aby uzyskać szczegółowe instrukcje, przykłady i uwagi dotyczące zobacz [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b265f-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="b265f-109">Zapisz witrynę jako szablon, polecenie nie jest obsługiwane i może być przyczyną problemów w witrynach, które używają publikowania infrastruktury serwera programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b265f-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="b265f-110">**Nie można utworzyć szablon witryny lub nie działa prawidłowo**</span><span class="sxs-lookup"><span data-stu-id="b265f-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="b265f-111">Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie aktywuje.</span><span class="sxs-lookup"><span data-stu-id="b265f-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="b265f-112">Jeśli funkcja nie jest dostępna uaktywnić w bieżącym zbiorze witryn, nie można użyć szablonu witryny do tworzenia witryny.</span><span class="sxs-lookup"><span data-stu-id="b265f-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="b265f-113">Sprawdź, jeśli list ani bibliotek przekraczają [Próg Limit widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 pozycji jak to zablokowanie tworzenia szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="b265f-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="b265f-114">Witryny mogą używać zbyt wiele zasobów i w związku z tym szablon witryny przekracza limit 50 megabajtów (MB).</span><span class="sxs-lookup"><span data-stu-id="b265f-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="b265f-115">Istnieją problemy z wyświetlaniem danych z listy, która jest używana kolumna odnośnika.</span><span class="sxs-lookup"><span data-stu-id="b265f-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="b265f-116">Aby uzyskać więcej informacji zobacz temat [generowany szablon listy nie są wyświetlane dane z listy wyszukiwania poprawne w dokumentacji Online programu SharePoint](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="b265f-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="b265f-117">Aby uzyskać szczegółowe informacje na temat typowych problemów i rozwiązań prosimy o odniesienie, [tworzenia i stosowania szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="b265f-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

