---
title: Utworzyć witrynę w dokumentacji Online programu SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199283"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="767bf-102">Tworzenie witryn programu SharePoint przy użyciu szablonów</span><span class="sxs-lookup"><span data-stu-id="767bf-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="767bf-103">Szablony witryn programu SharePoint są wbudowane definicje została zaprojektowana dla określonych potrzeb biznesowych.</span><span class="sxs-lookup"><span data-stu-id="767bf-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="767bf-104">Aby uzyskać więcej informacji zobacz [Używanie szablonów do tworzenia różnego rodzaju witryny programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="767bf-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="767bf-105">Poniżej przedstawiono typowe problemy/rozwiązania dotyczące zapisywania witryny lub listy jako szablonu w dokumentacji Online programu Sharepoint.</span><span class="sxs-lookup"><span data-stu-id="767bf-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="767bf-106">**Zapisz przycisk Szablon witryny/lista jest niedostępna lub Brak**</span><span class="sxs-lookup"><span data-stu-id="767bf-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="767bf-107">Administratorzy należy umożliwić niestandardowego skryptu do włączenia funkcji szablonu.</span><span class="sxs-lookup"><span data-stu-id="767bf-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="767bf-108">Aby uzyskać szczegółowe instrukcje Zobacz przykłady i uwagi</span><span class="sxs-lookup"><span data-stu-id="767bf-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="767bf-109">Zezwalanie lub blokowanie skryptu niestandardowego</span><span class="sxs-lookup"><span data-stu-id="767bf-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="767bf-110">Zapisz witrynę jako szablon, polecenie nie jest obsługiwane i może być przyczyną problemów w witrynach, które używają publikowania infrastruktury serwera programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="767bf-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="767bf-111">**Nie można utworzyć szablon witryny lub nie działa prawidłowo**</span><span class="sxs-lookup"><span data-stu-id="767bf-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="767bf-112">Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie aktywuje.</span><span class="sxs-lookup"><span data-stu-id="767bf-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="767bf-113">Jeśli funkcja nie jest dostępna uaktywnić w bieżącym zbiorze witryn, nie można użyć szablonu witryny do tworzenia witryny.</span><span class="sxs-lookup"><span data-stu-id="767bf-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="767bf-114">Sprawdź, jeśli list ani bibliotek przekraczają [Próg Limit widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 pozycji jak to zablokowanie tworzenia szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="767bf-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="767bf-115">Witryny mogą używać zbyt wiele zasobów i w związku z tym szablon witryny przekracza limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="767bf-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="767bf-116">Istnieją problemy z wyświetlaniem danych z listy, która jest używana kolumna odnośnika.</span><span class="sxs-lookup"><span data-stu-id="767bf-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="767bf-117">Aby uzyskać więcej informacji zobacz temat [generowany szablon listy nie są wyświetlane dane z listy wyszukiwania poprawne w dokumentacji Online programu SharePoint](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="767bf-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="767bf-118">Aby uzyskać bardziej szczegółowe informacje o typowe problemy i rozwiązania Sprawdź, czy [tworzenia i stosowania szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="767bf-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



