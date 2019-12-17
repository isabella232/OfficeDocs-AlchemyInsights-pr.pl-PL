---
title: Tworzenie witryny w programie SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052479"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="43610-102">Tworzenie witryn programu SharePoint przy użyciu szablonów</span><span class="sxs-lookup"><span data-stu-id="43610-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="43610-103">Szablony witryn programu SharePoint są wstępnie skompilowanymi definicjami zaprojektowanymi wokół konkretnej potrzeby biznesowej.</span><span class="sxs-lookup"><span data-stu-id="43610-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="43610-104">Aby uzyskać więcej informacji, zobacz [za pomocą szablonów do tworzenia różnych rodzajów witryn programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="43610-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="43610-105">Oto kilka typowych problemów/rozwiązań dotyczących zapisywania witryny lub listy jako szablon w programie SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="43610-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="43610-106">**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brak**</span><span class="sxs-lookup"><span data-stu-id="43610-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="43610-107">Administratorzy będą musieli zezwolić na skrypt niestandardowy, aby włączyć funkcje szablonu.</span><span class="sxs-lookup"><span data-stu-id="43610-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="43610-108">Szczegółowe kroki, przykłady i zagadnienia Zobacz</span><span class="sxs-lookup"><span data-stu-id="43610-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="43610-109">Zezwalanie lub zapobieganie skryptowaniu niestandardowym</span><span class="sxs-lookup"><span data-stu-id="43610-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="43610-110">Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy w witrynach, które korzystają z infrastruktury publikowania programu SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="43610-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="43610-111">**Nie można utworzyć szablonu witryny lub nie działa poprawnie**</span><span class="sxs-lookup"><span data-stu-id="43610-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="43610-112">Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie uaktywni się.</span><span class="sxs-lookup"><span data-stu-id="43610-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="43610-113">Jeśli funkcja nie jest dostępna do aktywowania w bieżącym zbiorze witryn, nie można użyć szablonu witryny do utworzenia witryny.</span><span class="sxs-lookup"><span data-stu-id="43610-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="43610-114">Sprawdź, czy wszystkie listy lub biblioteki przekraczają [próg limitu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 elementów, ponieważ może to blokować Tworzenie szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="43610-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="43610-115">Witryna może używać zbyt wielu zasobów i dlatego szablon witryny przekracza limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="43610-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="43610-116">Istnieją problemy z wyświetlaniem danych z listy, która używa kolumny odnośnika.</span><span class="sxs-lookup"><span data-stu-id="43610-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="43610-117">Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablon nie wyświetla danych z listy wyszukiwania poprawne w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="43610-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="43610-118">Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, należy sprawdzić [Tworzenie i używanie szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="43610-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



